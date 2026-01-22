# Expertise Matrix v30.2 — Strategic Intelligence Platform

This project is a specialized Strategic Leads Analysis platform designed for the telematics, logistics, and IoT industries. It integrates **Supabase** for real-time data management, **Groq (Llama 3.3 70B)** for deep analytical processing, and **Jina AI** for automated web research.

---

## 🧠 Core Intelligence Logic: "The Hierarchy of Truth"

To prevent AI hallucinations and ensure data integrity, the system operates on a strict anchoring principle:

1. **Primary Source (Internal Knowledge):** The AI treats existing notes in the `d` (Description) and `ai_strategic_summary` columns as the absolute truth. It is forbidden from contradicting this data during refinement.
2. **Secondary Source (Fresh Research):** When using the **Deep Check (Truck icon)**, Jina AI fetches live web data. This information is used solely to supplement missing facts or update volatile metrics (e.g., recent partnerships or revenue tiers), while respecting the primary source's domain.

---

## 📊 Strategic Analysis Framework

Every company analyzed by the system must adhere to a standardized 12-field JSON profile and a cohesive 2-sentence summary.

### The 6-Point Summary Requirement

Each strategic summary must explicitly cover:

1. **Business Model:** (e.g., Hardware Manufacturer, SaaS, Hybrid)
2. **Revenue Scale:** Based on defined financial tiers.
3. **Geographic Focus:** (e.g., EMEA, AMER, APAC, GLOBAL)
4. **Ecosystem Role:** (e.g., OEM, Tech Partner, Consumer)
5. **Software Strategy:** (Buy vs. Own Software R&D)
6. **Key Relationships:** Notable partners, parent companies, or major clients.

### Financial Scaling (Market Share Index)

* **LOW:** < $1 Billion (Niche players or emerging startups).
* **MID:** $1 Billion - $10 Billion (Established market leaders).
* **HIGH:** > $10 Billion (Global enterprise giants).

---

## 🛠 Technical Stack

| Component | Technology | Role |
| --- | --- | --- |
| **Database** | Supabase (PostgreSQL) | Real-time synchronization and persistent storage. |
| **LLM Engine** | Groq (Llama 3.3 70B) | Strategic reasoning, JSON structuring, and market analysis. |
| **Web Reader** | Jina AI | Markdown-optimized web scraping and research retrieval. |
| **Styling** | Tailwind CSS | Modern, responsive UI with "Diamond Mode" visualization. |

---

## ⚡ Key Features

### 📋 SSM (Similarity Scoring Methodology)

Calculates lead compatibility against a selected "Baseline" company:

* **SW Strategy Match:** +40%
* **Business Model Identity:** +30%
* **Ecosystem Role:** +15%
* **Market Share Alignment:** +10%
* **Domain Overlap:** +5%

### 💎 Hidden Diamonds Mode

A specialized view filter that isolates high-value opportunities. A "Diamond" is defined by:

* **Rapid Growth** + **Proprietary Software (Own SW: Yes)**
* **OR** a **Similarity Score (SSM) >= 80%**.

### 🪄 Sync & Refine

A one-click tool (`runAdvancedAnalysis`) that cleanses raw research notes into a polished, strategic executive summary without losing the original context.

---

## 🚀 Setup & Installation

1. **Database Configuration:** Ensure your Supabase table `companies` includes the necessary columns (`ai_strategic_summary`, `revenue_tier`, `growth_rate`, etc.).
2. **API Keys:** Open the Settings panel (⚙️) within the app to save your:
* `Groq API Key` (for AI Analysis).
* `Jina AI Token` (for Deep Web Research).


3. **Deployment:** The `index.html` is a standalone file that can be hosted on GitHub Pages, Vercel, or any static hosting provider.

---

## 🛡 Strategic Transparency

**Expertise Matrix v30.2** is a product of **Human-AI Co-Creation**.

* **Strategic Vision & Business Logic:** Defined by the Product Owner.
* **Algorithm Calibration & Code Execution:** Implemented in partnership with **Gemini & Llama 3.3**.

---

*Ref: LOG-MATRIX-2026-Q1 | Internal Use Only*
