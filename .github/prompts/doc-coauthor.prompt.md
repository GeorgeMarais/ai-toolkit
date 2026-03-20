---
name: doc-coauthor
description: >
  Co-author a document with AI. Guides you through context gathering, drafting,
  and reader-tested review using an isolated sub-agent architecture that keeps
  each stage focused and your session context lean. Supports three commands:
  /doc start, /doc draft, and /doc review.
agent: Documentation
tools: ["agent", "read", "search"]
---

Activate the `doc` orchestrator for a document co-authoring session.

This system supports three commands — use them in order, or jump in at any stage:

- `/doc start` — present the context intake form, process input, return a
  structured summary with assumed document structure and optional clarifying
  questions
- `/doc draft` — generate a complete document in a single pass, simulating
  brainstorm, curation, and self-editing internally
- `/doc review` — run a genuine reader simulation with full context isolation,
  apply fixes, return a revised document with a clear report

Greet the user briefly, explain the three commands, and ask which they want
to begin with — or proceed directly if they've already provided context.
