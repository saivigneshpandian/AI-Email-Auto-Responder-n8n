# 📧 AI FAQ Email Agent using n8n (RAG-Based Automation)

> AI-powered Gmail FAQ responder that retrieves answers from Google Drive documents using Retrieval-Augmented Generation (RAG) and automatically drafts email replies.

---

## 🚀 Overview

This project is an AI-driven email automation system built using **n8n**, **Google Gemini**, **Gmail API**, and **Google Drive API**.

When a user sends an email, the system:

1. Reads the incoming email
2. Retrieves relevant information from documents stored in Google Drive
3. Uses Gemini AI to generate a context-aware answer
4. Creates a draft reply automatically
5. Adds a label to organize the email thread

This simulates a real-world AI-powered customer support assistant.

---

## 🎯 Problem Statement

Organizations receive repetitive queries related to FAQs, policies, and documentation.

Manually searching documents and drafting responses:
- Wastes time
- Reduces efficiency
- Causes inconsistent answers

This project automates that workflow using AI-powered document retrieval.

---

## 🧠 Architecture (RAG Workflow)

The system follows a **Retrieval-Augmented Generation (RAG)** approach:

- 📥 Gmail Trigger → Detect new email
- 📩 Get Message → Fetch email content
- 📂 Google Drive → Retrieve relevant FAQ documents
- 🤖 Gemini AI Agent → Generate response using retrieved context
- 🧾 Structured Output Parser → Ensure clean formatted output
- ✍️ Create Draft → Auto-generate reply draft
- 🏷 Add Label → Organize email thread

---
## 🏗 Workflow Diagram

![Workflow Architecture]()

---
## 🛠 Tech Stack

- n8n (Workflow Automation)
- Google Gemini API
- Gmail API
- Google Drive API
- Structured Output Parsing
- JSON Workflow Architecture

---

## 📂 Project Structure


ai-faq-email-agent-n8n/
│
├── workflow.json                  # Exported n8n workflow
├── workflow-architecture.png      # Workflow diagram screenshot
└── README.md                      # Project documentation
---

## ⚙️ Setup Instructions

1. Clone this repository
2. Import the `workflow.json` file into your n8n instance
3. Configure the following credentials in n8n:
   - Gmail API
   - Google Drive API
   - Google Gemini API
4. Upload FAQ documents to Google Drive
5. Activate the workflow
6. Send a test email to trigger the system

---

## 🧪 Example Use Case

If a user sends an email asking:

"Can I get a refund for my subscription?"

The system:
- Retrieves refund policy from Google Drive
- Generates a context-based reply
- Creates a draft email response
- Labels the thread as "FAQ-Handled"

## 💡 Key Features

- AI-powered email query understanding
- Retrieval of relevant information from Google Drive documents
- Context-aware response generation using Gemini
- Automatic draft reply creation in Gmail
- Automatic email labeling for organization
- Structured JSON output handling

---

## 📈 Business Impact

- Reduces manual effort in answering repetitive FAQs
- Ensures responses are aligned with official documentation
- Improves response speed and consistency
- Demonstrates practical implementation of RAG architecture
- Scalable solution for customer support automation

---

## 🔮 Future Improvements

- Implement embedding-based vector search for better document retrieval
- Add confidence score for generated answers
- Add urgency detection and escalation logic
- Integrate with CRM systems
- Add analytics dashboard for tracking support trends

---

## 👨‍💻 Author

Built as part of AI Automation and Generative AI workflow experimentation using n8n.
