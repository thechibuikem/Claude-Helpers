# The "Make It Click" Learning Prompt

I am learning **[TOPIC]**.

I understand the basic definition/idea, but I struggle to build an accurate mental model of how it actually works.

Teach me in a way that **maps visually and intuitively**, rather than just giving me a formal explanation.

## Rules for your explanation

1. **Start with the concrete example, not the theory.**

   * Pick a small, realistic example.
   * Show the actual data/values involved.

2. **Use visual representations heavily.**

   * Use ASCII diagrams, number lines, tables, arrows, indexes, boxes, etc. wherever they help.
   * Make the visuals correspond directly to the code or concept.
   * For example:

   ```text
   0   1   2   3   4   5
   ↓   ↓   ↓   ↓   ↓   ↓
   A   B   C   D   E   F
           ↑
         middle
   ```

3. **Connect every important line of code to the visual.**
   Don't just say what this does:

   ```python
   low = mid + 1
   ```

   Show me visually WHY it becomes `mid + 1`.

   Explain what `+1` means in terms of positions, boundaries, or the actual data.

4. **Derive formulas instead of asking me to memorize them.**
   If you show me something like:

   ```python
   mid = low + (high - low) // 2
   ```

   first show me the intuitive version and derive the formula step-by-step from the idea.

5. **Explain WHY, not just WHAT.**

   Bad:

   > "`low = mid + 1` moves the lower bound."

   Good:

   > "We already checked `mid`, so it cannot be the answer. Therefore the next possible position is the position immediately after `mid`, which is `mid + 1`."

6. **Show the state changing step-by-step.**
   Use the same example through multiple iterations:

   ```text
   BEFORE
   low → [ ? ? ? ? ? ? ? ] ← high

   AFTER
   low → [ ? ? ? ] ← high
   ```

   Make it obvious exactly what was eliminated and why.

7. **Use plain English.**
   Avoid unnecessary jargon.
   If a technical term is necessary, define it immediately in simple language.

8. **Don't jump ahead.**
   If a concept depends on another concept, explain that piece first.

9. **Distinguish the mental model from the implementation.**
   Tell me:

   > "Here's what you should picture in your head."

   Then show how the code implements that mental model.

10. **Use counterexamples when useful.**
    Show me what would happen if I used the wrong value or wrong operation, and explain why it wouldn't work.

11. **At the end, give me a compact mental model.**
    Reduce the entire concept to a few rules I can remember.

## Most important requirement

I don't want an explanation that is merely technically correct.

I want an explanation where I can look at the code and think:

> **"Ohhh, I see why that line exists."**

If there is a piece of code that looks arbitrary, stop and visually derive **why it has to be written that way**.

Teach me like you're sitting beside me and drawing it out on a whiteboard.
