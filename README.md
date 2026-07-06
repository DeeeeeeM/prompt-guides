# 🧠 Context Engineering Prompt Master Template

This guide/template provides a **master template for building high-quality AI prompts** for coding assistants, repository analysis, and AI engineering workflows.

Instead of writing ad-hoc prompts, this framework helps you consistently construct structured, reliable, and production-grade AI instructions.

---

# 🚀 Overview

In context engineering, prompts are not written as single blocks.

They are **assembled from structured components**:

- Role
- Goal
- Context
- Constraints
- Inputs
- Output Format
- Workflow
- Guardrails

This ensures the AI behaves like a **controlled software component**, not a free-form chatbot.

---

# 🧠 Master Prompt Template

```text
ROLE
You are a senior software engineer and codebase analyst.

GOAL
[Define what success looks like]

CONTEXT
[Provide project overview, repository structure, documentation, etc.]

CONSTRAINTS
- [Rule 1]
- [Rule 2]
- Do not guess missing information
- Do not refactor unrelated code

INPUTS
[Paste file, repo tree, logs, or user request]

WORKFLOW
1. Understand the system
2. Identify relationships
3. Validate constraints
4. Propose solution
5. Only then suggest changes

OUTPUT FORMAT
[Define how the response should be structured]

GUARDRAILS
- If something is unclear, ask questions first
- Do not hallucinate missing files or behavior
- Prioritize correctness over speed

Current Free AI Engineering setup:

🧠 ChatGPT

→ context engineering + diff interpretation + planning

🏗 Claude

→ architecture + system design

💻 Claude coding

→ implementation

⚡ Cline

→ micro changes

📚 Git + docs

→ single source of truth

🔁 Context Packet (NEW KEY IDEA)

→ shared memory across all tools