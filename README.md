# AI-Powered IT Support Ticket Summarizer

This project automates the process of handling new IT support tickets by integrating **Airtable**, **OpenAI**, and **Gmail** within an `n8n` workflow.  
The goal is to generate concise, AI-powered summaries of incoming tickets and automatically send them to IT management for quicker decision-making.

---

## 🚀 Workflow Overview

1. **Airtable Trigger**  
   - Monitors a table for new incoming support tickets.  
   - Each new entry contains ticket details (description, priority, user, etc.).

2. **Message a Model (OpenAI)**  
   - Takes the raw support ticket information.  
   - Generates a **clear and concise summary** of the ticket.  
   - Focuses on important details for IT management (issue type, urgency, context).

3. **Send a Message (Gmail)**  
   - Automatically emails the summary to the IT management team.  
   - Ensures that management stays up-to-date without reading lengthy tickets.  

---

## 🛠️ Tech Stack

- [n8n](https://n8n.io/) – Workflow automation
- [Airtable](https://airtable.com/) – Ticket database
- [OpenAI API](https://platform.openai.com/) – AI text summarization
- [Gmail](https://workspace.google.com/products/gmail/) – Email notifications

---

## 📌 Benefits

- **Time-saving:** IT management no longer needs to read raw, unstructured tickets.  
- **Clarity:** Summaries highlight the most important issues.  
- **Automation:** No manual intervention required once set up.  

---

## ⚙️ Setup Instructions

1. Clone or replicate the workflow in your `n8n` instance.  
2. Configure Airtable credentials and set the trigger to watch your support tickets table.  
3. Set up your OpenAI API key in the **Message Model** node.  
4. Configure Gmail node with management’s email addresses.  
5. Activate the workflow.  
