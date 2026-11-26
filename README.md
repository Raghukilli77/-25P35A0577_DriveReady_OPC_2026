# -25P35A0577_DriveReady_OPC_2026
# 🤖 One Person Company — Agentic AI Workforce

Daily learning logs, code labs, and multi-agent systems built during the **12-Day Agentic AI Program (One Person Company)** organized by the **Department of Technical Training (DoTT), Aditya University** for 3rd-year DriveReady 8.0 students.

> **Goal:** Build a coordinated team of 3+ autonomous AI agents capable of running real-world business operations (Marketing, Operations, Sales & Support).

---

## 🛠️ Tech Stack & Tools
* **Language:** Python
* **Agent Orchestration:** LangGraph
* **LLMs & Inference:** Groq, Google Gemini
* **Memory & Vector Store (RAG):** ChromaDB
* **Protocol & Tooling:** Model Context Protocol (MCP)
* **Live Integrations:** Telegram, Gmail, Google Sheets

---

## 🗺️ 12-Day Program Roadmap

### Week 1: Online Foundations (`Nov 23 – Nov 28, 2026`)
*Focus: Agent foundations, tool calling, RAG, and LangGraph state machines.*

| Day | Date | Topic / Module | Status | Notes & Code |
| :--- | :--- | :--- | :---: | :--- |
| **Day 01** | Nov 23 | Introduction to Agentic AI & LLM Setup | ✅ | [View Notes](./Day-01/) |
| **Day 02** | Nov 24 | Tool Calling & Function Execution | ✅ | [View Notes](./Day-02/) |
| **Day 03** | Nov 25 | Your First Agent & LangChain / LangGraph Basics | ✅ | [View Notes](./Day-03/) |
| **Day 04** | Nov 26 | Agents with Memory & Knowledge (RAG + ChromaDB) | 🔄 | [View Notes](./Day-04/) |
| **Day 05** | Nov 27 | Multi-Agent Workflows & State Routing | ⬜ | [View Notes](./Day-05/) |
| **Day 06** | Nov 28 | MCP & External Integrations (Telegram, Gmail, Sheets) | ⬜ | [View Notes](./Day-06/) |

### Week 2: Offline Lab (`Nov 30 – Dec 5, 2026`)
*Focus: 80% hands-on full-day build of a production-ready AI workforce.*

* **Day 07 – Day 11 (`Nov 30 – Dec 4`):** Designing, building, and testing specialized agents:
  * 📢 **Marketing Agent:** Content generation, campaign outreach, and lead engagement.
  * ⚙️ **Operations Agent:** Order tracking, scheduling, and database/Sheets management.
  * 💬 **Sales & Support Agent:** Automated customer queries, reminders, and follow-ups via Telegram/Gmail.
* **Day 12 (`Dec 5, 2026`):** **Demo Day** — Live presentation to the industry jury.

---

## 📂 Repository Structure

```text
├── Day-01/                 # Daily notebooks, scripts, and markdown summaries
├── Day-02/
├── Day-03/
├── ...
├── capstone-project/       # Final Multi-Agent "One Person Company" source code
│   ├── agents/             # Marketing, Operations, and Sales/Support agent definitions
│   ├── tools/              # Custom Python tools, MCP servers, and API connectors
│   ├── rag/                # ChromaDB ingestion and retrieval scripts
│   └── main.py             # LangGraph orchestrator entry point
├── .env.example            # Template for Groq & Gemini API keys
├── requirements.txt        # Python dependencies
└── README.md
