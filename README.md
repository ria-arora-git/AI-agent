# 🧠 Autonomous Attendance Analyzer Agent

An AI-powered attendance chatbot built using **n8n**, Google Sheets, and Webhooks. Accepts natural language queries like “Was Rohan present today?” and replies instantly using structured data—no manual effort or prompting needed.

---

## 🚀 Features

- Fully automated—no buttons or UI required
- Google Sheets integration for real-time attendance
- Natural language support (via Webhook + custom Code node)
- Works 24/7, scalable across teams or institutions

---

## 📁 Project Structure

- `n8n-workflow.json` – Import this into n8n to get the full working flow
- `sample-attendance-sheet.csv` – Example data you can paste into Google Sheets

---

## ✅ Use Cases

- Schools: Students/Parents check if someone was present
- Teams: Managers quickly track remote attendance
- HR: Reduce repetitive attendance queries

---

## 🔮 Future Scope

- Add bulk queries like “Who all were absent today?”
- Integrate voice assistant support (Alexa, Google Assistant)
- Connect with biometric or QR-based systems
- Build real-time dashboards for attendance trends

---

## 📦 Setup

1. Import the workflow into n8n
2. Connect your Google Sheets node to a live sheet
3. Set your Webhook node to “Using Respond to Webhook node”
4. Deploy and activate

---

## 🤖 Example Query

```bash
curl -X POST https://yourdomain.n8n.cloud/webhook/your-workflow-id \
-H "Content-Type: application/json" \
-d '{"query": "Was Kabir Singh present today?"}'
