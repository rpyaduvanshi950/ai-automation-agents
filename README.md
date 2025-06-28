# 🧠 AI Agent Library by puspender

This repository provides a collection of powerful, ready-to-use AI agents designed for real business use, built in **n8n**—an open-source workflow automation tool. These agents automate tasks like email generation, lead scraping, and stock market analysis, helping you save time and boost productivity.

## ❓ What is n8n?
[n8n](https://n8n.io) is a free and open workflow automation tool that lets you connect different apps and automate repetitive tasks with no-code or low-code workflows. You can self-host it or use their cloud service.

---

## 🚀 Features
- **Pre-built workflows** (`.json` files) for instant import into n8n
- **Prompt engineering templates** for better AI results
- **Sticky Notes** for easy copy-paste into your n8n canvas
- **Step-by-step setup instructions** (see each agent's README)

---

## 🗂️ Agent Suite Overview

This repository features four powerful n8n agents: the Email Generator Agent for automated, personalized cold email outreach; the Lead Scraper Agent for extracting targeted leads from platforms like LinkedIn and Twitter into Google Sheets; the Stock Market Insights AI Agent for real-time stock data, news, and analysis; and Lead Scrapper 2, an advanced suite for high-volume lead scraping, enrichment, and research with a conversational interface. Together, these agents streamline business automation, lead generation, and market intelligence.

---

## 📋 Available Agents

Each agent now has its own detailed README with setup, usage, and customization instructions:

### 1. ✉️ [Email Generator Agent](./agents/email-generator-agent/README.md)
Generates cold emails from plain-text prompts, personalizes them, and sends automatically via Gmail.

### 2. 🕵️‍♂️ [Lead Scraper Agent](./agents/lead-scraper-agent/README.md)
Scrapes targeted leads from search terms and adds them to a Google Sheet.

### 3. 📈 [Stock Market Insights AI Agent](./agents/Stock-Market-Insights-AI-Agent/README.md)
Provides real-time stock market insights, news, and analysis from various sources.

### 4. 🧩 [Lead Scrapper 2](./agents/Lead-scrapper-2/README.md)
Advanced suite for high-volume lead scraping, enrichment, and research using Apollo.io, Relevance AI, and more. Includes a conversational agent for guided lead generation.

---

## 🛠 Prerequisites
- [n8n](https://n8n.io) installed (self-hosted or cloud)
- Google account (for Gmail/Sheets agents)
- API keys for any external services used in the workflows (see each agent's README)

---

## 🏁 How to Get Started

1. **Clone this repository**
   ```bash
   git clone https://github.com/rpyaduvanshi950/ai-automation-agents.git
   cd ai-agents
   ```
2. **Open n8n** (locally or in the cloud)
3. **Import the desired agent's `.json` file**
   - Go to n8n > Workflows > Import from File
   - Select the relevant `.json` file from the `agents/` subfolders
4. **Follow the agent-specific README**
   - Each agent folder contains a `README.md` with detailed setup and usage instructions.
5. **Activate the workflow** and start automating!

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
3. Add a `README.md` in your agent folder
4. Update this main README with your agent details
5. Open a pull request

---

## 📬 Contact & Tutorials
- For questions, open an issue or contact [puspender](mailto:puspender23@iitk.ac.com)
- 

BY Pushpender

