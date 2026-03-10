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

# 🚀 Workflow Diagram

<img width="1237" height="443" alt="image" src="https://github.com/user-attachments/assets/cfd61857-9b49-4a86-bca6-a125b9ea3cd3" />


# ⚙️ Technologies Used

- **n8n** – Workflow automation
- **Google Gemini 2.5 Pro** – AI architecture generation
- **Mermaid.js** – Diagram syntax
- **Kroki API** – Diagram rendering
- **Google Drive API** – File storage
- **Google Docs API** – Documentation logging

# 🧩 Workflow Overview

### 1️⃣ Chat Trigger
Receives architecture request from user.

Example:

Create AWS architecture with ALB, EC2 Auto Scaling and RDS


### 2️⃣ AI Agent (Gemini)

The AI agent acts as a **Senior Cloud Architect** and generates **Mermaid.js code** representing the architecture.

Example output:

<img width="983" height="862" alt="image" src="https://github.com/user-attachments/assets/5b6d9de0-6468-4e68-b75d-d16c6cb48747" />






### 3️⃣ Kroki API

Mermaid code is sent to:

https://kroki.io/mermaid/png

This API converts the Mermaid code into a **PNG architecture diagram**.

### 4️⃣ Google Drive

The generated diagram is uploaded automatically to a **Google Drive folder**.

### 5️⃣ Google Docs

A log entry is added to a Google Docs file containing:

- Timestamp
- Diagram link

This helps maintain **architecture documentation automatically**.


3️⃣ Configure credentials

Required credentials:

- Google Gemini API
- Google Drive OAuth
- Google Docs OAuth

# 💡 Example Prompts

Create a 3-tier architecture with load balancer, app servers and PostgreSQL database.

Create a Kubernetes cluster with ingress controller and microservices.

Create AWS architecture with ALB, EC2 Auto Scaling and RDS.

Create a GCP architecture with Cloud Run and Firestore.


# 🎯 Use Cases

• DevOps architecture design  
• Cloud solution design  
• Architecture documentation  
• AI-powered DevOps tools  
• Developer productivity automation  

# 👨‍💻 Author

*Ranjith Kumar*

DevOps Engineer | Cloud Automation | AI Workflows


---

# ⭐ If you like this project

Give it a ⭐ on GitHub!


