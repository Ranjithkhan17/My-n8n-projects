# 🤖 AI Agent Automation using n8n + Ollama + Telegram

An AI-powered automation system that generates motivational messages using a local LLM (Ollama), sends them to Telegram, and stores them in Google Sheets.

---

## 🚀 Overview

This project demonstrates how to:

- Use n8n AI Agent node
- Integrate Ollama (local LLM)
- Send automated Telegram messages
- Store results in Google Sheets
- Maintain memory to avoid repetition

---

## 🧠 Architecture

Schedule Trigger  
→ Set Topic  
→ AI Agent (Ollama)  
→ Telegram  
→ Google Sheets  

---

## 🔥 Features

- Fully local AI (No OpenAI cost)
- Automatic scheduling
- Memory buffer to avoid duplicate messages
- Google Sheets logging
- Telegram integration

---

## ⚙️ Requirements

- n8n (self-hosted or cloud)
- Ollama installed locally
- Telegram Bot
- Google Sheets account

---

## 🛠 Setup Instructions

### 1️⃣ Install Ollama

```bash
ollama pull llama3.2:1b
ollama run llama3.2:1b

📌 Learning Objectives

This project helps you learn:

n8n AI Agent configuration
Local LLM integration (Ollama)
Memory usage in AI workflows
Credential-safe template publishing
Automation portfolio building

👨‍💻 Author

Ranjithkumar
DevOps Engineer | AI Automation Enthusiast