# 🧠 AI Agent Library by Dharmik Solanki

This repository provides a collection of powerful, ready-to-use AI agents designed for real business use, built in **n8n**—an open-source workflow automation tool. These agents automate tasks like email generation, lead scraping, and stock market analysis, helping you save time and boost productivity.

## ❓ What is n8n?
[n8n](https://n8n.io) is a free and open workflow automation tool that lets you connect different apps and automate repetitive tasks with no-code or low-code workflows. You can self-host it or use their cloud service.

---

## 🚀 Features
- **Pre-built workflows** (`.json` files) for instant import into n8n
- **Prompt engineering templates** for better AI results
- **Sticky Notes** for easy copy-paste into your n8n canvas
- **Step-by-step setup instructions** (see below)

---

## 📋 Available Agents

### 1. ✉️ [Email Generator Agent](./agents/email-generator-agent)
- **What it does:** Generates cold emails from plain-text prompts, personalizes them, and sends automatically via Gmail.
- **Use cases:** Sales outreach, follow-ups, marketing campaigns.
- **Requirements:** Gmail account (for API access).
- **File:** `Email_Generation_agent.json`

### 2. 🕵️‍♂️ [Lead Scraper Agent](./agents/lead-scraper-agent)
- **What it does:** Scrapes targeted leads from search terms and adds them to a Google Sheet.
- **Use cases:** Lead generation, market research, contact list building.
- **Requirements:** Google Sheets account (for API access).
- **File:** `Lead_Scraper_Agent.json`

### 3. 📈 [Stock Market Insights AI Agent](./agents/Stock-Market-Insights-AI-Agent)
- **What it does:** Provides real-time stock market insights, news, and analysis from various sources.
- **Use cases:** Investment research, financial analysis, news aggregation.
- **Requirements:** May require API keys for certain data sources (see workflow notes).
- **File:** `Stock_Market_Insights_AI_Agent (1).json`

---

## 🛠 Prerequisites
- [n8n](https://n8n.io) installed (self-hosted or cloud)
- Google account (for Gmail/Sheets agents)
- API keys for any external services used in the workflows (see workflow notes)

---

## 🏁 How to Get Started

1. **Clone this repository**
   ```bash
   git clone https://github.com/dharmiksolanki/ai-agents.git
   cd ai-agents
   ```
2. **Open n8n** (locally or in the cloud)
3. **Import the desired agent's `.json` file**
   - Go to n8n > Workflows > Import from File
   - Select the relevant `.json` file from the `agents/` subfolders
4. **Configure credentials**
   - Set up Gmail, Google Sheets, or any other required credentials in n8n
   - Follow the notes inside each workflow for specific setup steps
5. **(Optional) Add Sticky Notes**
   - Copy the included Sticky Note text from the workflow and paste it into your n8n canvas for quick reference
6. **Activate the workflow** and start automating!

---

## 🧩 Example Use Case
- **Email Generator Agent:** Enter a prompt like "Write a cold email to introduce our new SaaS product to a marketing manager." The agent will generate and send a personalized email via your Gmail account.
- **Lead Scraper Agent:** Input a search term like "SaaS companies in New York" and the agent will populate a Google Sheet with relevant leads.
- **Stock Market Insights Agent:** Get the latest news and analysis for a specific stock symbol.

---

## ❓ Troubleshooting & FAQ
- **Import errors?** Make sure you are using a compatible version of n8n.
- **Credential issues?** Double-check that your Google/API credentials are set up correctly in n8n.
- **Missing data?** Review the workflow notes for required fields and API limits.
- **Still stuck?** Open an issue or reach out via the contact info below.

---

## 🤝 Contributing
Contributions are welcome! To add a new agent or improve existing ones:
1. Fork the repo
2. Add your `.json` workflow in a new or existing agent folder
3. Update this README with your agent details
4. Open a pull request

---

## 📬 Contact & Tutorials
- For questions, open an issue or contact [Dharmik Solanki](mailto:dharmiksolanki@gmail.com)
- Subscribe on [YouTube](https://www.youtube.com/@debugging_dost) for step-by-step video guides!

