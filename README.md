# 🚚 Expertise Matrix v30.3 — Strategic Intelligence Platform

**Expertise Matrix** is a high-performance Strategic CRM and Business Intelligence tool tailored for the logistics, telematics, and rail industries. It utilizes a **RAG (Retrieval-Augmented Generation)** architecture to transform raw web data into structured financial profiles and executive strategic summaries.

---

## 🧠 Architectural Core: Tavily + Groq RAG

In version 30.2, the platform has fully migrated from Jina AI to **Tavily AI**. This shift allows for multi-source research, aggregating data from financial news, LinkedIn, industry reports, and official corporate sites simultaneously.

1. **Tavily AI (Research Engine):** Acts as the "Field Researcher." It identifies facts regarding Revenue, EBITDA status, and business models across the live web.
2. **Groq (Llama 3.3 70B):** The central "Reasoning Engine." It analyzes retrieved data, compares it against existing internal knowledge, and structures it into valid JSON profiles.
3. **Supabase (Persistence):** A robust cloud database ensuring real-time synchronization of all strategic insights across the matrix.

---

## ⚡ Key Strategic Features

### 🪄 Sync & Refine (Strategic Executive Summary)

Generates a professional 6-point bulleted profile for any company:

* **Business Model:** (Hybrid / SaaS / HW)
* **Financials:** Exact Revenue figures and EBITDA margin status.
* **Geography:** Primary markets and global headquarters.
* **Ecosystem Role:** Position within the value chain (OEM, Platform, etc.).
* **Software Strategy:** Internal R&D focus vs. "Buy & Integrate" logic.
* **Ownership/Partners:** PE/VC backers, parent companies, and core strategic partners.

### 🚚 Deep Research (Automated Profiling)

Triggered by the "Truck" icon, this function automates the entire lead-entry process. By leveraging Tavily, the system now automatically detects and populates the **EBITDA Status** field, eliminating the need for manual financial digging.

### 📊 Flexible Similarity Scoring (SSM)

The "Look-alike" algorithm has been refined to understand "Hybrid" business models:

* **Hybrid Models** now receive a partial match score (+20%) when compared with pure-play hardware (**HW**) or software (**SaaS**) companies. This ensures high-relevancy targets are not filtered out due to rigid classification.

### 💎 Hidden Diamonds Mode

A specialized UI filter designed to isolate high-value opportunities:

* Identifies companies with **Rapid Growth** AND **Proprietary Software**.
* Flags any company with a **Similarity Match (SSM) ≥ 80%**.

---

## 🛠 Technical Stack

| Layer | Technology |
| --- | --- |
| **Frontend** | Vanilla JS, Tailwind CSS (Glassmorphism & Diamond UI) |
| **Database** | Supabase (PostgreSQL) |
| **Intelligence** | Groq API (Llama-3.3-70b-versatile) |
| **Research API** | Tavily Search AI (Advanced Search Depth) |

---

## 📜 Hierarchy of Truth (Data Integrity)

Version 30.2 implements the **Cumulative Knowledge** principle:
During every analysis, the AI treats the existing strategic summary as the "Absolute Truth" (Strategic Base). New web data is used only to supplement or update this base, ensuring that manually verified insights or high-quality previous reports are never overwritten by irrelevant web noise.

---

> **Project Meta:**
> * **Version:** 30.2 (Stable Build)
> * **Status:** Active Production / Operational
> * **Co-Creation:** Strategic Vision by Product Owner; Technical implementation by Gemini & Llama 3.3.
> 
