# ⚔️ Competitor Analysis: Actual Budget

This file contains a detailed, citation-backed teardown of **Actual Budget**, a highly popular open-source, privacy-first personal and micro-business budgeting tool.

---

## 📌 Specific Product Name
*   **Product Name:** Actual Budget
*   **Developer:** Open-Source Community (originally founded by James Long, open-sourced in 2022).
*   **Hosting Model:** Local-first web app (runs in-browser with local SQLite database) or self-hosted server via Docker.

---

## 📋 Feature List
*   **Envelope Budgeting:** Enforces zero-based envelope budgeting where every dollar is allocated to a specific category [2][3].
*   **Local-First Architecture:** Keeps all transaction data in a local SQLite file in the browser or on the desktop, enabling absolute offline capability [2][7][8].
*   **End-to-End Encrypted (E2EE) Sync:** Encrypts data before uploading to a custom sync server, guaranteeing that not even the hosting server can view your financial records [2][7].
*   **Financial Reports:** Visual analytics showing monthly spending trends, net worth tracking, and cash flows [1][4][3].
*   **Optional Bank Sync:** Links bank feeds through third-party APIs (SimpleFIN in US/Canada or GoCardless in Europe) [2][5].

---

## 💰 Price
*   **Core Software:** **$0.00 / Free** (Open-Source under MIT License) [2][6][3].
*   **Hosting Sync Server:** Free if self-hosted locally or via personal servers (e.g. Synology, Raspberry Pi) [2][6][3]; ~$1.50 / month if using low-cost managed cloud hosting like PikaPods [5][6].
*   **Bank Sync API:** ~$15.00 / year if using SimpleFIN in the US [2][5]; free or low-cost for GoCardless in select European regions.
*   **Citations:** Actual Budget Official Project Site and GitHub Documentation, 2026.

---

## 🎯 Target Audience
*   **Primary Users:** Privacy-conscious individuals, developers, tech-savvy solopreneurs, and micro-business owners who use envelope-style budgeting (YNAB refugees) and want full control of their records [4][3][8].

---

## 🎨 User Experience (UX)
*Visual Reference:* ![Actual Budget Web UI](file:///f:/AIML%20projects/solo-accounting/3_competitive_research/screenshots/actual_budget.png)

*   **UI Analysis:** Actual Budget is built with a stunning, modern, and clean minimalist aesthetic:
    *   Fully integrated sleek dark mode support.
    *   Clean, color-coded envelope category bars showing budgeted vs. actual balances.
    *   A fluid grid system that responds instantly with zero loading spinners.
*   **UX Strengths:** Extremely fast, modern, and beautiful. Navigating categories and entering transactions feels incredibly satisfying.
*   **UX Weaknesses:** Initial Docker/managed server setup for enabling cloud sync is highly technical and requires software familiarity [3][8].

---

## ⭐️ User Ratings and Reviews
*   **Overall Sentiment:** Exceptionally high praise across Reddit finance forums and GitHub star trends:
    *   **Privacy & Sync Quality:** Highly rated for offering bulletproof End-to-End Encryption, allowing users to sync between phone and computer without compromising data [7][3].
    *   **Cost Efficiency:** Viewed as the premier alternative to YNAB (which charges over $100/yr) [2][4][5].
*   **Key Con Sentiment:**
    *   **Technical Setup Barrier:** Setting up the sync server requires some technical comfort with Docker, node, or managed hosting configurations, which is intimidating for average consumers [3][8].
    *   **No Native Mobile App:** Relies on a Progressive Web App (PWA) wrapper rather than a fully compiled native App Store application.
*   **Citations:** Github stars, Reddit Self-Hosted & Personal Finance communities, and Actual Budget reviews (2026).
