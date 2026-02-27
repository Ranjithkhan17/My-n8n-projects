# 🏋️ AI Personal Productivity + Habit Tracker (n8n + Ollama)

An AI-powered personal productivity and health tracking system built using:

- n8n
- Ollama (Local LLM)
- Telegram Bot
- Google Sheets

---

## 🚀 Overview

This workflow allows users to send natural language updates via Telegram like:

Workout: yes  
Sugar: 140  
Study: n8n  
Minutes: 50  
Content: no  
Notes: Interview preparation  

The system:

1. Uses Ollama (local LLM) to extract structured data
2. Converts AI output into valid JSON
3. Stores daily records in Google Sheets
4. Automatically formats timestamp (IST)

---

## 🧠 Workflow_daigram

<img width="1251" height="486" alt="architect_daigram" src="https://github.com/user-attachments/assets/ddde31e5-086a-4b0b-a211-639af6f9d2dc" />


---

## 📊 Google Sheet Structure

| Date | Workout | Sugar | Study Topic | Study Minutes | Content | Notes |
|------|---------|-------|------------|--------------|---------|-------|

---

## ⚙️ Setup Instructions

### 1️⃣ Install Ollama

```bash
ollama pull llama3.2:1b
ollama run llama3.2:1b

Ensure Ollama is running locally.

🧪 Example Input
Workout: yes
Sugar: 150
Study: LLM
Minutes: 45
Content: no
Notes: Interview preparation

🎯 Features

AI-based natural language parsing

Automatic JSON validation

Type-safe numeric conversion

IST timezone formatting

Fully local LLM (no OpenAI cost)

👨‍💻 Built By

Ranjithkumar
DevOps Engineer | AI Automation Enthusiast
