---
name: denny-office-brief
description: Prepare a project assignment for Denny Office or a Denny Agents coding session, with a bounded scope, dependencies and observable acceptance criteria. Use when the user wants to turn a request into an Office поручение or split work between agents. Do not activate for unrelated planning.
---

# Denny Office Brief

Turn the user's request into a brief that a person can paste into an Office project or agent chat. This package produces documents; it does not create Office records or start agents.

Read the request and the project material the user supplied. When a repository is available and relevant, inspect its instructions and the few entry points needed to understand the change. Preserve requirements already settled in the conversation. Ask only about missing decisions that would change the scope or outcome; mark other unknowns explicitly.

Use [the assignment template](assets/assignment.md) as a starting point, shortening it for small tasks. Include:

- The concrete problem and desired behavior, including a before/after example when useful.
- Included work and boundaries. Name the actual repository, branch or working directory only when known.
- A small set of acceptance criteria a reviewer can observe, not statements such as “make it good.”
- Relevant files or links, their purpose, and the source of uncertain facts.
- Appropriate validation and the evidence the agent should return.
- The human decision needed when a result is ready for review.

When splitting work, give each assignment a distinct owner or leave the owner unassigned. Identify shared files and dependencies. Do not assign two agents overlapping mutations in the same working tree without a coordination plan. An independent review assignment should state what it reviews and what it may change.

Return a ready-to-paste brief in the user's language. If the user asks for a file, save it at their chosen location or a clearly named new file in the current workspace; avoid overwriting an existing brief. Do not say a task was submitted, accepted by an agent, or queued in Office unless an independently available authorized integration actually confirmed that action. Installing this skill provides no such integration.
