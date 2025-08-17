# Client Feedback Analyzer (n8n + AI Automation)

This project is an end-to-end client feedback automation system built with **n8n**.  
It collects client feedback (NPS ratings & comments), analyzes it using AI, and automatically triggers account management actions to improve client retention.

---

## 🎥 Demo Video  
👉 [Watch the Demo](https://drive.google.com/file/d/1rJqZa7c2GhoOGN9t6HiobdeovZRTR5vM/view?usp=sharing)

---

## ⚡ Features

- **Feedback Collection**: Captures client feedback via a webhook (NPS 1–10, name, ID, comments).  
- **AI Analysis**: Uses an AI agent to analyze comments and check for improvement opportunities.  
- **Smart Notification Rules**:
  - If *scope for improvement only* → alert sent to **Account Manager**  
  - If *NPS ≤ 6* → alerts sent to both **CX** and **Account Manager**  
- **Context-Rich Updates**: Every notification includes:
  - The last 4 NPS scores of the client  
  - The latest client comment  
  - A summary of all past comments  
- **One-Click Actions for Managers**:
  - Raise a ClickUp ticket  
  - Book a Calendly call with the client  
  - Ignore feedback if not relevant  
- **Automated Updates**: Feedback and alerts are logged in Google Sheets and sent instantly to managers/teams.  
- **Human-in-the-Loop**: Combines automation with manager decisions to keep oversight in client handling.  

---

## 🛠️ Tech Stack

- **n8n** – Workflow automation platform  
- **OpenAI API** – For natural language processing and summarization  
- **Google Sheets API** – For structured record keeping  
- **ClickUp API** – For ticket creation  
- **Calendly API** – For client meeting booking  

---

## 📂 Workflow Overview  

Here’s a snapshot of the workflow in n8n:  
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/19e9569e-e4cc-4f99-938d-47f45a80fcee" />

---

## 🚀 How It Works  

1. Client feedback is submitted via **Webhook**.  
2. The **AI Agent** analyzes comments and interprets sentiment/improvement scope.  
3. **Notification logic runs**:  
   - Scope for improvement only → Alert to Account Manager  
   - NPS ≤ 6 → Alerts to both CX and Account Manager  
4. Alerts include:  
   - The last 4 NPS ratings from the client  
   - The most recent comment  
   - A summary of all past comments  
5. Account Manager gets **actionable options**:  
   - Create a ClickUp ticket  
   - Book a Calendly call  
   - Ignore if not relevant  
6. System updates logs and notifies stakeholders in **real-time**.  

---

## 🌟 Why This Project Matters  

- Saves time by eliminating manual feedback checks  
- Provides **context-rich insights** (not just raw data)  
- Makes client retention **proactive, not reactive**  
- Ensures at-risk clients are never missed  
- Creates a balance between **automation** and **human decision-making**  

---

## 📬 Contact  

Created by **Bhomik**  

💼 [LinkedIn](www.linkedin.com/in/bhomik-verma)  
📧 Email: **Bhomik183@gmail.com**
