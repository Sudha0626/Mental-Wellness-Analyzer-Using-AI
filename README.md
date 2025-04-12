# Mental-Wellness-Analyzer-Using-AI

```markdown
# 🧠 Mental Wellness Diary Analyzer

This project is a LangChain-based application designed to help users analyze their daily journal entries and receive motivational feedback. It uses an open-source LLM (Mistral-7B-Instruct) via Hugging Face and is built using [Langflow](https://astra.datastax.com/langflow).

---

## 🎯 Objective

Allow users to:
- Input daily emotional journal entries.
- Receive an **emotional tone analysis**, **recurring themes**, and **personalized motivational tips**.

---

## ⚙️ Tech Stack

- **Langflow** (visual chain building for LangChain)
- **Hugging Face Inference API**
- **Mistralai/Mistral-7B-Instruct-v0.3** (open-source LLM)
- Optional: **Streamlit** for final UI (deployment-ready)
  
---

## 🛠️ Functional Overview

### 🔹 User Input
- Simple **Text Input** or **Chat Input** component in Langflow.
- Users write their daily emotional experiences.

### 🔹 LLM Prompt
Prompt sent to LLM:
```
Analyze the following journal entry: {journal_entry}. 
Determine the emotional tone, identify recurring themes, 
and provide personalized motivational advice.
```

### 🔹 Output
- **Emotional Analysis**
- **Themes/Sentiments**
- **Personalized Motivational Tips**

---

## 🚀 How to Run

###  1. Clone & Setup

```bash
git clone https://github.com/your-username/mental-wellness-diary-analyzer.git
```

Make sure you have access to [Langflow via Astra](https://astra.datastax.com/langflow).

###  2. Import Langflow Project

- Open Langflow.
- Click `Import Flow` → upload the provided `.json` file (Langflow export).

###  3. Configure Components

- **Model**: Choose `Hugging Face > Mistralai/Mistral-7B-Instruct-v0.3`
- **API Key**: Paste your Hugging Face API Token inside the HuggingFace component.

###  4. Connect the Flow

- Input → Prompt Template → Hugging Face Model → Output
- Set `journal_entry` as the variable name inside the Prompt Template.

###  5. Run it!

- Click **Playground**.
- Enter journal text.
- Get emotional analysis + tips!

---

##  Future Enhancements

- Export journal history & trends.
- Sentiment score charts.
- Streamlit UI deployment on Hugging Face Spaces.
- Mental wellness resources integration.

---


## 🤝 Acknowledgements

- [Mistral AI](https://huggingface.co/mistralai)
- [Hugging Face](https://huggingface.co)
- [Langflow](https://astra.datastax.com/langflow)

---

## 💬 Feedback

Feel free to raise issues or contribute via pull requests!

```
