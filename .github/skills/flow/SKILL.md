---
name: flow
description: Create a user flow from a confirmed requirement Markdown file and save it in .flow-kit/flows.
---

# Flow

Create a user flow grounded in a specific requirements document.

## Process

1. Identify the requirement Markdown file the user wants to use. If it is not clear, ask for its path; do not create a flow from an unspecified requirement.
2. Read the requirement file before designing the flow. If it is missing or does not provide enough information, explain what is missing and ask one focused question at a time.
3. Map the relevant actors and starting conditions through the primary user journey to its outcome. Include meaningful decisions, alternate paths, validation failures, and recovery paths supported by the requirement.
4. Do not add behavior that the requirement does not support. Mark necessary but unresolved details as open questions instead of guessing.
5. Create `.flow-kit/flows/` if it does not exist. Save the flow as Markdown using the requirement's feature slug (for example, `.flow-kit/flows/invite-members.md`). If that file already exists, choose a distinct filename or ask before replacing it.
6. Include the source requirement path, a concise purpose, actors and preconditions where applicable, and the flow steps. Use a Mermaid flowchart when it makes branching easier to understand; make sure its labels agree with the written steps.
7. Tell the user the path to the created file.
