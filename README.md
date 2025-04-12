# 🧠 Mental Wellness Diary Analyzer

This project is a LangChain-based application designed to help users analyze their daily journal entries and receive motivational feedback. It uses an open-source LLM (Mistral-7B-Instruct) via Hugging Face and is built using [Langflow](https://astra.datastax.com/langflow).

---

##  Objective

Allow users to:
- Input daily emotional journal entries.
- Receive an **emotional tone analysis**, **recurring themes**, and **personalized motivational tips**.

---

##  Tech Stack

- **Langflow** (visual chain building for LangChain)
- **Hugging Face Inference API**
- **Mistralai/Mistral-7B-Instruct-v0.3** (open-source LLM)
- Optional: **Streamlit** for final UI (deployment-ready)
  
---

##  Functional Overview

###  User Input
- Simple **Text Input** or **Chat Input** component in Langflow.
- Users write their daily emotional experiences.

###  LLM Prompt
Prompt sent to LLM:

LangFlow using Astra:
1. Import Langflow Project
Open Langflow.

Click Import Flow → upload the provided .json file (Langflow export).

2. Configure Components
Model: Choose Hugging Face > Mistralai/Mistral-7B-Instruct-v0.3

API Key: Paste your Hugging Face API Token inside the HuggingFace component.

3. Connect the Flow
Input → Prompt Template → Hugging Face Model → Output

Set journal_entry as the variable name inside the Prompt Template.

4. Run it!
Click Playground.
Enter journal text.
