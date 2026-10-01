# Agent team

The custom agent team for building Mona's Project Pulse dashboard:

- **Planner** — Target model: Claude Opus 4.7 (copilot). Researches the repository and produces an implementation plan, including dependencies, edge cases, and validation expectations. Definition: `.github/agents/planner.agent.md`.
- **Designer** — Target model: Gemini 3.1 Pro (copilot). Defines the dashboard's UX, accessibility, information hierarchy, interactions, and visual design. Definition: `.github/agents/designer.agent.md`.
- **Coder** — Target model: GPT-5.5 (copilot). Implements the assigned application code and support files, with explicit errors and validation. Definition: `.github/agents/coder.agent.md`.
- **Orchestrator** — Target model: Claude Opus 4.7 (copilot). Coordinates the specialists, plans task phases and file ownership, and verifies the integrated result without implementing it. Definition: `.github/agents/orchestrator.agent.md`.

I am using GitHub Copilot CLI in a Codespace to orchestrate the work.
