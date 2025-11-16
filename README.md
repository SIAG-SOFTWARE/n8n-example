🧩 SIAG Software — n8n Example Workflow

This repository provides a minimal, clean workflow example built for n8n.
Its goal is to serve as a quick reference for clients and developers evaluating SIAG Software’s automation capabilities.

🔧 What this example does

A simple two-step automation:

HTTP Request → Fetch a sample TODO item from a public API.

Google Sheets Append → Write the received data into a Google Sheet.

This mirrors a common real-world automation pattern:
collect → transform → store.

📊 Diagram — Basic Workflow
HTTP Request  ───►  Google Sheets Append


And here is the visual version:

📁 Files Included
```
n8n-example/
│
├── example_workflow.json   # Full n8n workflow (import directly into n8n)
└── docs/
    └── diagram_basic.png   # Visual diagram of workflow
```
🧪 How to Use

Open your n8n instance

Go to Workflows → Import

Upload example_workflow.json

Replace the sheetId with your own Google Sheet

Add Google credentials in n8n if required

🧠 Why this exists

This is a minimal educational example used for:

client onboarding

demonstrating workflow structure

testing n8n installations

explaining API → Sheet automations in consulting sessions

For a real production-grade example, see:

👉 n8n-workflows-advanced (your other repo)

📬 Contact

SIAG Software
AI Automation • Chatbots • Full-Stack Development
📧 siag.software@protonmail.com
