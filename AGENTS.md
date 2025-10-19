# AGENTS.md  
Guidelines and context for AI coding agents contributing to CodeHub.

## 🧭 Project Overview
CodeHub is a brand-new, open-source platform for hosting, collaborating on, and deploying code. It aims to be a lightweight, modular, and self-hostable alternative to GitHub and GitLab with a strong community ethos.

If you're an autonomous coding agent working within this repository, everything you do should support the early-stage goals of the project:
- Build the Minimum Viable Product (MVP)
- Keep the architecture modular and developer-friendly
- Preserve openness, clarity, and extensibility

## 🗂️ Repository Structure (Expected)

/codehub
├─ src/              ← backend & service logic
├─ web/              ← frontend UI
├─ docs/             ← specifications and design notes
├─ tests/            ← test suites
├─ scripts/          ← tooling & setup scripts
├─ README.md         ← human developer intro
└─ AGENTS.md         ← this file

*(If folders don’t exist yet, agents should create them when contributing code.)*

## ✅ Agent Responsibilities
- Write clean, modular code with descriptive names
- Add comments only where necessary—avoid noise
- Follow existing patterns when extending functionality
- Include or update tests when relevant
- Never introduce external services without justification

## 🛠️ Tech Stack (Proposed Defaults)
Until changed in project documentation, assume:
- **Backend:** Node.js (TypeScript) or Go
- **Frontend:** React or Svelte
- **Database:** PostgreSQL
- **CI/CD:** YAML-based pipeline definitions
- **Containerization:** Docker

If a decision must be made and no human instructions exist, prefer:
1. Simplicity
2. Modularity
3. Open-source friendliness

## ⚙️ File & Commit Conventions
- Use `kebab-case` for filenames (e.g., `user-service.ts`)
- Use `snake_case` for config files
- Use `PascalCase` for classes/types
- Use commit messages in the form:
  - `feat: ...`
  - `fix: ...`
  - `docs: ...`
  - `refactor: ...`
  - `test: ...`

## 🤖 When Unsure
Agents should:
1. Check existing docs or code conventions
2. Prefer minimal viable implementations
3. Leave `// TODO:` or `// QUESTION:` comments when clarification is needed

## 🌱 Early Priorities for Agents
1. Establish skeleton repo structure
2. Create minimal backend service entrypoint
3. Draft initial API mock
4. Set up CI config and Dockerfile
5. Scaffold basic frontend placeholder

## ❌ Things to Avoid
- Overengineering or premature abstractions
- Adding dependencies just for convenience
- Implementing speculative features not in MVP scope
- Creating files outside the expected structure

## ✅ Definition of Done (Agent Tasks)
A task is considered complete when:
- Code compiles
- Tests (if applicable) pass
- The feature integrates without breaking existing files
- Relevant docs or TODOs are updated

---

This document may expand as CodeHub evolves. Until then, follow these guidelines to keep contributions coherent and on-track.
