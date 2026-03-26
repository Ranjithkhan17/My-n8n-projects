🚀 LogDoctor AI – Intelligent Linux Log Analyzer
🧠 Overview

LogDoctor AI is an AI-powered DevOps automation workflow built using n8n that analyzes Linux system logs and automatically generates actionable insights and remediation reports.

It helps engineers quickly identify issues like:

🔐 Security attacks (SSH brute-force)
💾 Disk space issues
🌐 Network failures
⚙️ Service crashes

⚡ Features
🔍 AI-based log analysis (Google Gemini / LLM)
🧠 Root cause detection
🚨 Severity classification (Low → Critical)
🛠️ Auto-generated fix suggestions
🛡️ Preventive recommendations
📄 Automated report generation in Google Docs
🔄 Fully automated workflow (Webhook-based)


🏗️ Architecture


🧪 Sample Input

📤 Sample Output

Video refrence

----------------------------------------------------------
⚙️ Setup Instructions

1. Import Workflow
Open n8n
Import provided JSON workflow

2. Configure Credentials
Add Google Docs OAuth2 credentials
Add Gemini / OpenAI API key

3. Start Webhook
POST /webhook/logs

4. Send Logs
echo "Mar 26 10:15:22 server kernel: EXT4-fs warning (device sda1): ext4_dx_add_entry: Directory index full!
Mar 26 10:15:23 server systemd[1]: Failed to start Docker Application Container Engine.
No space left on device" | curl -X POST http://localhost:5678/webhook-test/logs -H "Content-Type: text/plain" --data-binary @-

-----------------------------------------------------------
🚀 Use Cases
DevOps Monitoring
Incident Response Automation
Security Analysis
SRE Operations
Freelancing automation product
----------------------------------------------------------
👨‍💻 Author

Ranjithkumar
DevOps Engineer | Automation Enthusiast
⭐ If you like this project, give it a star!
----------------------------------------------------------

