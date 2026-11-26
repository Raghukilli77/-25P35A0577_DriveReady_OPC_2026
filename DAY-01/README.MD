# Day 01 — Groq LLM Setup, System Prompts & Prompt Guard

**Repository:** `25P35A0577_DriveReady_OPC_2026`  
**Notebook:** [`daY-01/day1.ipynb`](https://colab.research.google.com/github/Raghukilli77/-25P35A0577_DriveReady_OPC_2026/blob/main/daY-01/day1.ipynb)

---

## Overview
First hands-on session covering Groq API integration in Google Colab using `langchain_groq` and the native `groq` SDK, structured system prompt design, and prompt-injection detection.

## What Was Built & Tested
1. **Environment & API Setup:** Installed `langchain_groq` and configured `GROQ_API_KEY` securely via Google Colab `userdata` secrets.
2. **Deterministic Chat Inference:** Initialized `ChatGroq` with `openai/gpt-oss-120b` (`temperature=0`) for consistent, rule-bound responses.
3. **System Prompt Engineering:** Built a domain-specific assistant (*Sweet Crumbs Home Bakery*) enforcing business facts, strict negative constraints (no delivery time promises), tone rules, and a 60-word limit.
4. **Input Safety Guardrail:** Tested `meta-llama/llama-prompt-guard-2-22m` to score adversarial jailbreak/prompt-injection inputs (`0.9989` injection confidence).

## Tech Stack
* **Platform:** Google Colab (Python 3)
* **Libraries:** `langchain-groq`, `groq`
* **Models:** `openai/gpt-oss-120b`, `meta-llama/llama-prompt-guard-2-22m`
