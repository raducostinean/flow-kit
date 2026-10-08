---
name: to-story
description: Turn a user flow Markdown file into implementation-ready user stories and save them in .flow-kit/stories.
---

# To Story

Translate a provided flow into a small, coherent set of user stories with implementation details.

## Process

1. Identify the flow Markdown file the user wants to use. If it is not clear, ask for its path; do not create stories from an unspecified flow.
2. Read the flow file and any requirements document it explicitly references. If the source is missing or too ambiguous to derive stories, explain the gap and ask one focused question at a time.
3. Split the flow into independently implementable user stories that together cover its supported paths. Express each story from the relevant user's perspective and include:
   - A concise title and user-story statement.
   - Acceptance criteria in observable, testable terms, including relevant alternate or failure paths.
   - Implementation notes grounded in the flow or requirements, including dependencies and data or system behavior when specified.
4. Keep implementation notes actionable without inventing architecture, APIs, or technology choices. Mark unresolved decisions as open questions.
5. Create `.flow-kit/stories/` if it does not exist. Save the stories as Markdown using the flow's feature slug (for example, `.flow-kit/stories/invite-members.md`). If that file already exists, choose a distinct filename or ask before replacing it.
6. Include the source flow path and, when available, the referenced requirements path. Tell the user the path to the created file.
