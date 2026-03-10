# 🧠 AI Cloud Architecture Diagram Generator (n8n + Gemini + Kroki)

This project demonstrates how to automatically generate **cloud architecture diagrams using AI**.

Users simply describe infrastructure in natural language, and the system generates a **professional architecture diagram automatically**.

Example input:

Create a web application with a load balancer and three web servers connected to a database.

The workflow will:
1. Convert the prompt into **Mermaid architecture code**
2. Render it as a **diagram**
3. Upload it to **Google Drive**
4. Log the result in **Google Docs**

---

# 🚀 Architecture

User Prompt  
↓  
n8n Chat Trigger  
↓  
Gemini 2.5 Pro (AI Agent)  
↓  
Mermaid Diagram Code  
↓  
Kroki API (Diagram Rendering)  
↓  
PNG Architecture Diagram  
↓  
Google Drive Upload  
↓  
Google Docs Documentation

---

# ⚙️ Technologies Used

- **n8n** – Workflow automation
- **Google Gemini 2.5 Pro** – AI architecture generation
- **Mermaid.js** – Diagram syntax
- **Kroki API** – Diagram rendering
- **Google Drive API** – File storage
- **Google Docs API** – Documentation logging

---

# 🧩 Workflow Overview

### 1️⃣ Chat Trigger
Receives architecture request from user.

Example:

Create a web app with load balancer, 3 web servers and a MySQL database.

---

### 2️⃣ AI Agent (Gemini)

The AI agent acts as a **Senior Cloud Architect** and generates **Mermaid.js code** representing the architecture.

Example output:





---

### 3️⃣ Kroki API

Mermaid code is sent to:

https://kroki.io/mermaid/png

This API converts the Mermaid code into a **PNG architecture diagram**.

---

### 4️⃣ Google Drive

The generated diagram is uploaded automatically to a **Google Drive folder**.

---

### 5️⃣ Google Docs

A log entry is added to a Google Docs file containing:

- Timestamp
- Diagram link

This helps maintain **architecture documentation automatically**.

---

3️⃣ Configure credentials

Required credentials:

- Google Gemini API
- Google Drive OAuth
- Google Docs OAuth

---

# 💡 Example Prompts

Create a 3-tier architecture with load balancer, app servers and PostgreSQL database.

Create a Kubernetes cluster with ingress controller and microservices.

Create AWS architecture with ALB, EC2 Auto Scaling and RDS.

Create a GCP architecture with Cloud Run and Firestore.

---

# 🎯 Use Cases

• DevOps architecture design  
• Cloud solution design  
• Architecture documentation  
• AI-powered DevOps tools  
• Developer productivity automation  

---

# 👨‍💻 Author

**Ranjith Kumar**

DevOps Engineer | Cloud Automation | AI Workflows

GitHub: https://github.com/YOUR_GITHUB

---

# ⭐ If you like this project

Give it a ⭐ on GitHub!


