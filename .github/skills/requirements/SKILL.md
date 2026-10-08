---
name: requirements
description: Interview a user to clarify an app feature or product requirement, then save the agreed requirements as a Markdown file in .flow-kit/requirements.
---

# Requirements

Turn the user's idea into a clear, actionable requirements document by interviewing them before writing it.

## Interview

- Ask exactly one concise question per turn. Do not combine questions, ask a multi-part question, or present a questionnaire.
- Start with the most important unknown about the user's goal. Use each answer to choose the next question.
- Clarify the intended users, problem and desired outcome, scope, expected behavior, acceptance criteria, important edge cases, and constraints as needed. Skip points the user has already answered.
- Keep interviewing until the requirement is specific enough to implement. If an answer is ambiguous or contradictory, ask one question to resolve it.
- Do not write the requirements file while important details remain unclear. When enough is known, briefly confirm the understood scope and ask for correction only if necessary.

## Write the requirement

Once the user has provided enough information:

1. Create `.flow-kit/requirements/` if it does not exist.
2. Write a Markdown file named with a short, lowercase, hyphen-separated slug of the feature (for example, `.flow-kit/requirements/invite-members.md`).
3. Include a descriptive title and the confirmed problem, users, goals, functional requirements, acceptance criteria, and relevant constraints or edge cases. Omit sections that do not apply; do not invent details.
4. If a file with that name already exists, avoid overwriting it. Choose a distinct filename or ask the user which file to update.
5. Tell the user the path to the created file.
