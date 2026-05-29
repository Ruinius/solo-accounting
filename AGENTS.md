# Solo Accounting - Repository Index & Agent Guidelines

Welcome, AI Agent! This file outlines the repository structure, documentation practices, and development standards for **Solo Accounting** (a free or low-cost accounting solution).

> [!IMPORTANT]
> **Pre-Coding Check:** ALWAYS read this file (`AGENTS.md`) before writing any new code or creating/editing documentation in this repository. This ensures alignment with existing structures, documentation indexes, and design decisions.

---

## 📂 Project Directory Structure

```text
solo-accounting/
├── .gitignore                      # Git ignore rules for OS, editors, and temporary files
├── AGENTS.md                       # [THIS FILE] Core index, standards, and AI guidelines
├── README.md                       # Main landing page and quick entry dashboard
├── mission_vision/                 # Tactically guiding mission and long-term vision
│   ├── mission.md                  # The mission statement
│   └── vision.md                   # The vision statement
├── user_research/                  # Target personas and market pain points
│   └── user_research_summary.md    # Synthesis of user research, stories, and workflows
├── competitive_research/           # Direct and indirect competitive analysis
│   └── competitive_research_summary.md # Summary of competitors, pricing models, and market gaps
├── product_spec/                   # Product requirements and MVP definition
│   └── product_spec_summary.md     # Summary of product features and roadmap
├── architecture/                   # Technical architecture plans and data storage design
│   └── architecture_summary.md     # Technical stack, local-first philosophy, and privacy
├── ai_agents/                      # Multi-agent coordination and workspace setup
│   └── ai_agents_summary.md        # Summary of agent prompt guidelines and tools
└── business_model/                 # Financial modeling and pricing strategy
    └── business_model_summary.md   # Pricing tiers, operational cost projections, and value
```

---

## 📘 Documentation Guidelines & Standards

To ensure a highly professional and readable repository, all markdown files must adhere to the following rules:

1. **Rich & Harmonious Typography:**
   * Use GitHub-flavored alerts (`> [!NOTE]`, `> [!TIP]`, `> [!IMPORTANT]`, etc.) to emphasize crucial takeaways.
   * Maintain consistent spacing and header hierarchy (`#` -> `##` -> `###`).
2. **Aesthetic & Responsive Layouts:**
   * Break up dense information into scannable lists, tables, or Mermaid diagrams when explaining workflows or processes.
   * Do not use generic placeholders; keep all documentation detailed and production-ready.
3. **Continuous Index Updates:**
   * If a new file is added or a file is renamed/deleted, **IMMEDIATELY** update the file structure map above.
   * If new documentation topics are introduced, update the corresponding `summary.md` in that folder to keep it accurate.
4. **Environment Compatibility:**
   * This workspace runs on a **Windows** environment. Commands and shell interactions must use PowerShell (`pwsh`) syntax.
   * Use `uv` for any Python-related scripting or automation helpers that may be added to the project.

---

## 🤖 AI Agent Guidelines

As a pair programmer and business plan developer in this repo, follow these instructions:
* **Plan Before Execution:** Use planning mode artifacts (`implementation_plan.md`, `task.md`, `walkthrough.md`) for any non-trivial modifications.
* **Keep Summaries Updated:** Each directory (except `mission_vision/`) must have a corresponding summary markdown file that provides a high-level view of the files inside that directory.
* **Data Ownership Focus:** The core USP of Solo Accounting is local-first, privacy-respecting, low-cost/free utility. Ensure all architectural and product decisions respect these principles.
