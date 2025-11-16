SIAG n8n Example Workflow

A minimal example workflow demonstrating how SIAG Software uses n8n for automation, data extraction and integration pipelines.

This example includes:

✔️ A basic HTTP request

✔️ Writing data into Google Sheets

✔️ A clean JSON format ready for import

✔️ Simple, beginner-friendly automation
```
📁 Files included
n8n-example/
├── example_workflow.json   → Import directly into n8n
└── README.md
```
🚀 Usage
1. Open n8n

Self-hosted or Cloud version both work.

2. Import the workflow

Go to:
n8n → Workflows → Import From File → select example_workflow.json

3. Configure nodes

Replace SHEET_ID with your Google Sheets ID

Connect your Google OAuth credentials

Run the workflow

🧪 What this workflow does

1️⃣ Fetches a test JSON resource:
https://jsonplaceholder.typicode.com/todos/1

2️⃣ Extracts id and title

3️⃣ Appends the result into Google Sheets:

ID	Title
1	delectus aut autem
📝 Notes

This is a minimal SIAG workflow for demonstration.

For production-level pipelines, see
👉 n8n-workflows-advanced (multi-step, scraping, notifications, architecture diagram, etc.)

📄 License

MIT — SIAG Software

```
   ┌─────────────────┐
   │  HTTP Request    │
   │  (Fetch JSON)    │
   └─────────┬───────┘
             │
             ▼
   ┌─────────────────┐
   │ Google Sheets    │
   │ (Append Row)     │
   └─────────────────┘
```
