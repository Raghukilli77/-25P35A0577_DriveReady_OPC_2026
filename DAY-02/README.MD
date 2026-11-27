# 📅 Day 02 — System Prompts, Guardrails & Conversational Chatbot

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Raghukilli77/-25P35A0577_DriveReady_OPC_2026/blob/main/DAY-02/day02.ipynb)

Hands-on lab from **Day 02** of the **One Person Company (Agentic AI Program)** at Aditya University (DoTT). Focuses on using the OpenAI-compatible SDK with Groq, enforcing strict system role constraints, and building a stateful CLI business assistant with sliding-window memory and API error handling.

---

## 🎯 Key Concepts Covered
* **Groq OpenAI-Compatible Client:** Connecting to `https://api.groq.com/openai/v1` using the `openai` Python SDK and `openai/gpt-oss-120b`.
* **Secure Secret Retrieval:** Fetching `GROQ_API_KEY` from Google Colab `userdata` with environment variable and `getpass` fallbacks.
* **System Prompt Engineering & Guardrails:**
  * Restricting model behavior (e.g., enforcing a quote-maker persona that declines joke requests).
  * Structuring prompts using `ROLE`, `FACTS`, `RULES`, and `FORMAT` blocks to prevent hallucinations (`"I'll check with the owner."`) and enforce response length/language rules (English/Telugu).
* **Sliding-Window Conversation Memory:** Maintaining chat state via a `history` list while slicing recent messages (`MAX_TURNS`) alongside the system prompt to manage token usage.
* **Error Handling & Logging:** Handling `RateLimitError` and `APIConnectionError` gracefully, plus a `@log_call` decorator (`functools.wraps`) on a `get_price` helper function.

---

## 🧪 Notebook Breakdown (`day02.ipynb`)
1. **Setup & Role Enforcement:** Installs `openai`, configures the Groq client, tests system prompt boundaries (*quote maker vs. joke maker*), and inspects token usage (`CompletionUsage`).
2. **Sweet Crumbs Home Bakery Assistant:** An interactive CLI loop (`chat()`) that answers customer queries against a fixed rupee menu (`plum cake`, `chocolate cake`, `cupcake`), enforces 24-hour order notice rules, and exits cleanly on `bye`, `exit`, or `quit`.

---

## 🚀 How to Run
1. Click the **Open In Colab** badge above.
2. Add `GROQ_API_KEY` to your Google Colab **Secrets** (🔑 icon on the left sidebar) or enter it when prompted.
3. Run all cells
