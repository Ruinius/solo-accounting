# 🤖 AI Agent Guidelines Summary - Solo Accounting

This directory outlines the AI agent framework that drives and automates the operations of the **Solo Accounting** business. Instead of just in-app features, these agents act as virtual team members to keep development fast, support responsive, and customer acquisition highly cost-effective.

---

## 📂 Business Operations Agents Dashboard

We have defined five distinct, highly specialized AI agents to manage different domains of the Solo Accounting business:

| Agent Name | Core Mandate | Primary Channels / Tools | Specification |
| :--- | :--- | :--- | :--- |
| **📞 Customer Service** | Strict anti-hallucination support answering and ticket routing. | Support Email, Ticketing Database | [customer_service_agent.md](file:///f:/AIML%20projects/solo-accounting/6_ai_agents/customer_service_agent.md) |
| **🛠️ Issue Resolution** | Nightly batch runs to resolve low-risk bug tickets. | Git, Local Sandbox Test Env | [issue_resolution_agent.md](file:///f:/AIML%20projects/solo-accounting/6_ai_agents/issue_resolution_agent.md) |
| **🗺️ Roadmap** | Aggregates feedback to maintain minor queue & propose major specs. | Feedback Parser, Backlog Manager | [roadmap_agent.md](file:///f:/AIML%20projects/solo-accounting/6_ai_agents/roadmap_agent.md) |
| **💻 Coding** | Nightly automated feature implementation & sandbox testing. | Compiler, Linter, Git PR | [coding_agent.md](file:///f:/AIML%20projects/solo-accounting/6_ai_agents/coding_agent.md) |
| **📣 Marketing** | Benign, organic, value-first small business community building. | Reddit, Social Media API | [marketing_agent.md](file:///f:/AIML%20projects/solo-accounting/6_ai_agents/marketing_agent.md) |

---

## 🔄 Multi-Agent Operations & Synergies

To run the Solo Accounting business at near-zero operational overhead, these five agents operate in a continuous, cooperative loop:

```mermaid
graph TD
    A[Marketing Agent attracts Users] --> B[Users send support emails]
    B --> C[Customer Service Agent answers or opens Ticket]
    C -- Bug Ticket --> D[Issue Resolution Agent patches bug at 02:00 AM]
    C -- Feature Request --> E[Roadmap Agent aggregates request into minor queue]
    E --> F[Coding Agent implements feature at 03:00 AM]
```

1. **Information Flow:** User feedback collected by **Customer Service** is analyzed by the **Roadmap Agent**, which directly updates the queue for the **Coding Agent**.
2. **Schedule Separation:** Execution times are staggered to prevent database and repository locks (Bug fixes run at **02:00 AM**, Feature additions run at **03:00 AM**).
3. **Safety & Quality Gateways:** All engineering activities (Bug Fixes and Coding) require 100% test coverage and linter verification before any code hits production.