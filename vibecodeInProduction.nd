# Engineering Workflow and Operating Standards

## 1. Start with Docs, Not Code
- First write `README.md`: clear project definition, architecture overview, plain-English explanation, repository structure, and helpful diagrams.
- Then write `SETUP.md`: step-by-step environment setup instructions for Linux, macOS, and Windows with exact commands and no assumed prior installs.
- Then create a requirements and task-breakdown document: functional requirements categorized by priority (MUST and SHOULD) grouped by feature, followed by a granular task breakdown including owner, dependencies, specific steps, acceptance criteria, and files to create. This serves as the shared team task list.

## 2. Build Stage by Stage, One Task at a Time
- Implementation proceeds strictly one task at a time based on user direction.
- Provide full code for the active task in chat: every required file delivered in order, accompanied by a concise explanation detailing why it is built this way.
- Explicitly state the target folder and branch before writing any code.
- If a task depends on an unfinished task, identify the dependency immediately and suggest robust stubbing strategies to prevent blocking.

## 3. I Run Things, You Diagnose
- Diagnostics rely on real terminal output and actual error logs pasted by the user.
- Analyze from explicit output data; never guess or assume a fix resolved an issue without user confirmation.
- If an error breaks downstream steps such as local infrastructure state, partial writes, or duplicated data, provide clear, explicit instructions on how to undo the change cleanly.

## 4. PR Description After Each Task
- Once a task's implementation is confirmed working, generate a professional pull request title and description.
- Include a summary of changes, file-by-file breakdown, verification steps based on actual confirmed tests rather than assumptions, and specific notes for reviewers.

## 5. Standards
- Use plain English across all documentation, keeping sentences short and avoiding unnecessary jargon.
- Flag any technical inaccuracies, inconsistencies, or overclaimed features immediately, including within requirement documents, rather than smoothing them over.
- Never use em dashes in any written document.
- Keep folder structures flat and task-named unless there is a strong architectural reason to nest.
