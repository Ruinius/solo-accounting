# 🤖 AI Agent Guidelines Summary - Solo Accounting

This directory defines the operational frameworks, coding standards, and collaborative patterns for **AI Agents** (such as Antigravity) working on the Solo Accounting project. It also conceptualizes how AI capabilities will be integrated directly into the product itself.

---

## 🛠️ Operational Rules for Collaborating Agents

To maintain perfect alignment, every AI agent working in this workspace must adhere to the following workflow regulations:

```text
┌────────────────────────┐      ┌────────────────────────┐      ┌────────────────────────┐
│  1. READ AGENTS.md     │ ───> │  2. PLANNING MODE      │ ───> │  3. MODULAR EXECUTION  │
│  Consult folder index  │      │  Draft implementation  │      │  Write pristine code   │
└────────────────────────┘      └────────────────────────┘      └────────────────────────┘
```

1. **The Pre-Coding Directive:**
   * Before writing a single line of code or modifying documentation, you **MUST** read [AGENTS.md](file:///f:/AIML%20projects/solo-accounting/AGENTS.md).
   * Ensure you are fully aware of module boundaries and avoid duplicating existing documentation structures.

2. **PowerShell & Windows First Compatibility:**
   * This repository operates on a **Windows** system. All terminal tasks and command propositions must strictly use PowerShell (`pwsh`) syntax.
   * Path operations must handle backslashes correctly (`\`) or be absolute URIs.

3. **Modern Python Tooling via `uv`:**
   * If creating helper scripts, financial forecasting modules, or data generators in Python, always use **`uv`**.
   * Run commands using `uv run python <script.py>`. Never use `pip` or standard `venv` activations directly.

4. **Premium Visual Guidelines:**
   * Any UI components created must be stunning at first glance. Use harmonious color palettes, fluid transitions, and sleek styling.
   * Do not write placeholder text. Keep everything fully formed, professional, and functional.

---

## ⚡ Agentic UI: Embedded AI Features

In addition to dev-time rules, Solo Accounting will feature **Agentic UI** capabilities built directly into the client. AI agents will assist the user within the interface:

### 1. Natural Language Command Bar
Instead of clicking through multi-layered menus, a Command Bar (e.g., `Ctrl + K`) allows users to speak in plain English:
* *User input:* "Create an invoice for Sarah Design for 800 dollars due in 2 weeks"
* *Agent action:* Parses the intent, queries the client directory, compiles the invoice draft, and presents it to the user for single-click approval.

### 2. Intelligent Auto-Categorization Agent
* When bank statements are uploaded, an agent analyzes transaction names against historical logs and business types to suggest ledger account classifications.
* *Confidence scoring:* Displays high-confidence matches silently, but flags low-confidence matches with a gentle visual highlight for user confirmation.

### 3. Smart Tax Estimation Agent
* Monitors ongoing earnings and expenses, cross-references with local tax structures, and runs predictive simulations to advise users on how much to reserve for quarterly estimated taxes.
