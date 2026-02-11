
## 🤖 AI Agent Automation using n8n, Ollama & Telegram

Production-ready AI Agent workflow built with n8n. Demonstrates Agentic AI, local LLM integration (Ollama), chat memory, Telegram bot automation, and Google Sheets logging.

## 📌 Project Overview

This project showcases an AI-powered automation workflow built using n8n that:

✅ Runs on a scheduled trigger  
✅ Uses a local LLM (Ollama) via an AI Agent  
✅ Maintains conversation memory to avoid repetition  
✅ Sends AI-generated responses (motivational quotes) to Telegram  
✅ Logs every interaction into Google Sheets


## 🧠 Workflow Architecture

![Workflow Diagram]https://github.com/Ranjithkhan17/My-n8n-projects/blob/main/AI_Agents_Messenger/workflow_diagram.png

### Workflow Nodes:

1. **Schedule Trigger1** - Executes every 10 seconds
2. **Edit Fields** - Prepares topic list for AI processing
3. **AI Agent** - Generates motivational message using Ollama
4. **Ollama Chat Model** - Local LLM integration (llama3.2:1b)
5. **Simple Memory** - Maintains conversation context
6. **Send a text message** - Delivers message to Telegram
7. **Append row in sheet** - Logs message to Google Sheets

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| **Automation** | n8n (Docker – self-hosted) |
| **AI / LLM** | Ollama (Local LLM) |
| **Agent Framework** | n8n AI Agent |
| **Messaging** | Telegram Bot |
| **Storage** | Google Sheets API |
| **Memory** | n8n Simple Memory Buffer |
| **Runtime** | Docker |

---

## 📋 Prerequisites

Before using this workflow, you need:

- **n8n** instance running (Docker or self-hosted)
- **Ollama** installed and running locally with `llama3.2:1b` model
- **Telegram Bot** created (via @BotFather on Telegram)
- **Google Sheets API** enabled with credentials
- Basic knowledge of n8n workflow setup

---

## 🚀 Setup Instructions

### Step 1: Prepare the Template

1. Copy `Motivational_AI_agents.json.template` 
2. Rename to `Motivational_AI_agents.json`
3. Replace all placeholders with actual values

### Step 2: Get Your Credentials

#### Ollama Setup
```bash
# Start Ollama service
ollama serve

# In another terminal, pull the model
ollama pull llama3.2:1b
```

#### Telegram Bot Setup
1. Chat with @BotFather on Telegram
2. Create a new bot and get your **API Token**
3. Get your **Chat ID** (use @userinfobot or your personal chat ID)

#### Google Sheets Setup
1. Go to [Google Cloud Console](https://console.cloud.google.com)
2. Enable Google Sheets API
3. Create OAuth 2.0 credentials
4. Get your **Google Sheet ID** from the URL

### Step 3: Import and Configure in n8n

1. Open your n8n instance
2. Import the JSON file
3. Update credentials for each node:
   - Ollama Chat Model
   - Telegram Bot
   - Google Sheets API

### Step 4: Test the Workflow

1. Click "Execute Workflow" to test manually
2. Check Telegram for the motivational message
3. Verify data was logged in Google Sheets
4. Enable the workflow to run on schedule

---

## 📁 Project Structure


AI_agents_messenger/
├── README.md                              # This file
├── workflow_diagram.png                   # Visual workflow architecture
├── Motivational_AI_agents.json            # ⚠️ PRIVATE - Original
├── Motivational_AI_agents.json.template   # ✅ PUBLIC - Safe template


## 🧪 Testing & Troubleshooting

### Issues & Solutions

| Issue | Solution |
|-------|----------|
| Ollama not responding | Verify Ollama is running |
| Telegram message not sent | Check Chat ID and Bot Token |
| Google Sheets not logging | Verify API credentials |

---

## 📊 Customization

### Change AI Model
Edit Ollama Chat Model node to use a different model

### Modify Topics
Edit Edit Fields node to update topics array

### Change Schedule
Edit Schedule Trigger1 node to adjust interval

---

## 👨‍💻 Author

**Ranjithkumar**  
Automation Engineer | DevOps | AI Workflow Builder

🔗 [GitHub Profile](https://github.com/Ranjithkhan17)

---

**Last Updated:** February 2026  
**Status:** ✅ Production Ready 
>>>>>>> df3ea9a (Motivational AI_agents)




