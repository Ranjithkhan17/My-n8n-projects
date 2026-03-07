# 🏢 ERP Order Processing & Regional Reporting Automation (n8n)

This workflow automates ERP order processing, customer data enrichment, regional filtering, file generation, and multi-channel notifications.

---

## 🚀 Overview

This automation:

1. Fetches order data from ERP system via HTTP API
2. Fetches customer data from Airtable
3. Merges order and customer data
4. Sorts orders by price
5. Filters by region (Americas)
6. Generates JSON & CSV reports
7. Sends email with attachment
8. Sends Discord notifications

---

## 🧠 Workflow_diagram
<img width="1378" height="641" alt="image" src="https://github.com/user-attachments/assets/993e4641-ce21-409f-924d-36252c7a6f73" />

### High-Value Orders Path:
→ Convert to JSON File  
→ Send Email (Gmail)  
→ Discord Notification  

### All Orders Loop Path:
→ Split in Batches  
→ Format Fields  
→ Convert to CSV  
→ Discord Notification  

---

## 🔥 Key Features

- Multi-source data integration
- Data merging using key mapping
- Conditional regional filtering
- High-value order detection
- Automated email attachments
- Discord status notifications
- Batch processing support
- Date formatting automation

---

## ⚙️ Required Credentials

You must configure:

- HTTP Header Authentication
- Airtable Personal Access Token
- Gmail OAuth2
- Discord Webhook

---

## 📊 Data Processing Logic

### Step 1: Fetch ERP Orders
Orders are retrieved via secured HTTP API call.

### Step 2: Fetch Customer Records
Customer metadata is retrieved from Airtable.

### Step 3: Merge Data
Join performed using:

customerID (Orders)  
CustomerID (Airtable)

### Step 4: Sort Orders
Sorted by `orderPrice` in descending order.

### Step 5: Filter by Region
Only records where:

region = "Americas"

are processed for high-value path.

---

## 📁 File Generation

Two file types generated:

- JSON (Individual Order Files)
- CSV (Batch Export Files)

---

## 📧 Notifications

- Gmail: Sends file attachments
- Discord: Sends status message with order ID reference

---

## 🧩 Customization Ideas

- Add Slack integration
- Add CRM update
- Add automatic invoicing
- Add analytics dashboard
- Deploy on production server

---

## 🎯 Learning Objectives

This workflow demonstrates:

- Advanced n8n merge logic
- Conditional branching
- Batch processing
- Multi-channel notification system
- Enterprise-level automation patterns

---

## 👨‍💻 Author

Ranjithkumar  
DevOps Engineer | Automation Specialist  
