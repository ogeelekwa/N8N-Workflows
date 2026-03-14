 This collection of workflows of my personal automations, ranging from **Agentic RAG systems** to **Voice AI** and **Lead Qualification**.

Here is a structured `README.md` you can use for your repository. It categorizes your workflows and highlights the tech stack for each, making it easy for others (or your future self) to understand the setup.

---

# 🚀 Advanced n8n AI Automation Library

A curated collection of production-ready **n8n workflows** focusing on Agentic AI, Retrieval-Augmented Generation (RAG), and seamless API integrations.

## 📂 Workflow Directory

| Workflow | Key Features | Tech Stack |
| --- | --- | --- |
| **Ultimate Personal Assistant** | A "Master Agent" that orchestrates sub-workflows for email, calendar, and research. | OpenRouter, Tavily, Telegram |
| **Agentic RAG Template** | Automated document ingestion from Google Drive into a vector database. | Supabase, OpenAI, Google Drive |
| **AI Job Application Tracker** | Aggregates job postings from 10+ sources (RSS/APIs) into Google Sheets. | Indeed, LinkedIn, Glassdoor, Adzuna |
| **Technical Analyst Agent** | Analyzes stock market charts via Telegram and provides technical insights. | GPT-4o, Anthropic, Chart-Img API |
| **Telegram Voice Agent** | Full speech-to-speech AI interaction loop. | ElevenLabs, OpenRouter, Telegram |
| **Outbound Lead Qualifier** | Automated phone qualification for new form leads. | Vapi AI, Google Sheets, JS Standardizer |
| **Travel Agent** | Generates comprehensive travel itineraries with flights and resorts. | SerpApi, Tavily, Claude 3.5, Gmail |
| **Supabase/Postgres RAG** | Modular backend for storing and retrieving vectorized data. | Supabase, OpenAI Embeddings |

---

## 🛠️ Getting Started

### 1. Import Workflows

To use these workflows, download the desired `.json` file and:

1. Open your n8n instance.
2. Create a new workflow.
3. Click the **three dots (⋮)** in the top right → **Import from File**.
4. *Alternatively:* Open the JSON file in a text editor, copy the code, and **Paste** (`Ctrl+V`) directly onto the n8n canvas.

### 2. Configure Credentials

**Note:** n8n does not export sensitive API keys. You will need to set up your own credentials for:

* **LLMs:** OpenAI, Anthropic, or OpenRouter.
* **Storage:** Supabase, Postgres, and Google Sheets.
* **Communication:** Telegram Bot API, Gmail, and Vapi.
* **Search:** SerpApi and Tavily.

### 3. Environment Variables

Some workflows utilize specific Node IDs or Webhook URLs. Ensure you update any **Execute Workflow** nodes to point to the correct sub-workflow IDs within your own n8n instance.

---

## 💡 Highlights

### Agentic RAG Pipeline

The `Agentic RAG AI Agent Template` is designed for scale. It automatically detects new PDFs or Spreadsheets in a Google Drive folder, extracts text, and updates a **Supabase Vector Store**. The agent can then answer complex questions across your entire document library.

### Voice AI Integration

Using `Telegram Voice Agent`, you can send voice notes to your bot. It transcribes your voice, processes the intent through an LLM, and responds with a high-fidelity cloned voice using **ElevenLabs**.

---

## 📄 License

This repository is open-source. Feel free to fork, modify, and use these workflows in your own projects.

---
