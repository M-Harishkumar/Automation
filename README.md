# 💡 Automation – AI-Powered Financial Tracker

This project automates personal finance tracking using n8n, AI models, and Google Sheets. It intelligently detects bank transaction messages, classifies them (credit/debit), extracts details, and stores them in structured sheets. It also visualizes profit/loss with charts—no code required.

## 🚀 Features

- 📩 Auto-detects SMS or Email transaction alerts
- 🧠 Uses AI to classify credit/debit transactions
- 🗂️ Extracts data: amount, description, date, vendor, category
- 📊 Automatically adds entries to Google Sheets
- 🧾 Generates dynamic charts (e.g. monthly profit vs. loss pie chart)
- 🔒 100% privacy – works on your own infrastructure

## 📦 Tech Stack

- ⚙️ n8n (workflow automation)
- 📧 IFTTT (to capture SMS or emails)
- 📊 Google Sheets (as a financial database)
- 🤖 AI Model (text classification + information extraction)

## 📈 Example Use Case

You receive a bank message like:
A/c *3515 Debited for Rs:500.00 on 02-08-2025 13:34:43 by Mob Bk ref no 558092309549 Avl Bal Rs:558.69.

The workflow will:

1. Detect it's a debit.
2. Extract:
   - Amount: ₹500.00  
   - Description: Mobile Banking Transaction  
   - Vendor: Union Bank  
   - Date: 2025-08-02  
   - Category: Debit  
3. Store it in Google Sheets.
4. Update monthly loss chart.

## 🛠️ Setup Instructions

1. Clone this repo.
2. Set up n8n on your machine/cloud.
3. Connect IFTTT to Gmail or SMS and forward messages to webhook.
4. Configure Google Sheets credentials.
5. Import the n8n workflow JSON (provided in this repo).
6. Start the workflow!

## 📌 Project Goal

To help non-coders automate financial record-keeping with minimal setup, using the power of AI and no-code tools.

---

📬 Feel free to fork, contribute, or ask for help in the Issues section.
