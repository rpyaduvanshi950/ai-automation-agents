# 🕵️‍♂️ Lead Scraper Agent

## Overview
The Lead Scraper Agent is an AI-powered workflow for n8n that automates the process of finding and extracting targeted leads from the web (e.g., LinkedIn, Twitter) and saving them to Google Sheets. It uses AI to interpret your search intent, scrapes results via SerpAPI, and structures the data for easy outreach.

---

## Features
- Converts plain-language search requests into structured queries
- Scrapes Google search results (e.g., LinkedIn profiles) using SerpAPI
- Extracts names, roles, companies, LinkedIn URLs, and snippets
- Saves leads to Google Sheets for easy access
- **Supports multiple lead scraper types (LinkedIn, Twitter, or generic web search)**
- Optional: Integrate with email automation for outreach

---

## Lead Scraper Types
The agent supports different types of lead scraping, allowing you to target specific platforms or perform a general search:

- **LinkedIn Scraper**: Finds leads from LinkedIn profiles. Use prompts like "Scrape LinkedIn for marketing managers."
- **Twitter Scraper**: Finds leads from Twitter profiles. Use prompts like "Scrape Twitter for SaaS founders."
- **Generic Scraper**: Performs a broader search across the web for the specified roles. Use prompts like "Find AI experts online."

The workflow automatically detects the platform from your prompt and builds the appropriate search query:
- For LinkedIn: `site:linkedin.com/in ("role1" OR "role2")`
- For Twitter: `site:twitter.com ("role1" OR "role2")`
- For generic: Just the roles or keywords

### Example Prompts for Each Type
```
Scrape LinkedIn for product managers in Bangalore. Give me 15 leads.
Scrape Twitter for AI founders. Give me 10 leads.
Find growth hackers online. Give me 5 leads.
```

---

## How It Works
1. **Trigger**: The workflow starts with a chat or webhook trigger where you input a search request (e.g., "Scrape LinkedIn for AI founders in New York. Give me 20 leads.").
2. **Parse Request**: An LLM node converts your request into a structured JSON (platform, roles, lead count, filters, location).
3. **Build Search Query**: The workflow builds a Google search query targeting the desired platform and roles.
4. **Scrape Results**: SerpAPI fetches search results, focusing on LinkedIn/Twitter profiles or generic web results.
5. **Extract Lead Data**: The workflow parses each result to extract name, role, company, LinkedIn/Twitter URL, and snippet.
6. **Save to Google Sheets**: All leads are appended to a connected Google Sheet.

---

## Required Credentials
- **SerpAPI**: API key for web scraping
- **Google Sheets**: OAuth2 credentials for saving leads
- **OpenRouter/OpenAI**: API key for LLM nodes

---

## Step-by-Step Setup
1. **Import the Workflow**: In n8n, import `Lead_Scraper_Agent.json` from this folder.
2. **Configure Credentials**:
   - Add your SerpAPI key as an HTTP credential in n8n.
   - Set up Google Sheets OAuth2 and select it in the Sheets node.
   - Add your OpenRouter or OpenAI API key for the LLM nodes.
3. **Prepare Your Google Sheet**:
   - Create a sheet with columns: Name, Role, Company, LinkedIn URL, Snippet, Scraped At.
   - Link the sheet in the workflow.
4. **Trigger the Workflow**:
   - Use the chat/webhook trigger or run manually.
   - Enter a search prompt (see above for examples).
5. **Review Results**:
   - Leads will be added to your Google Sheet automatically.

---

## Tips & Customization
- Adjust the search query logic for different platforms or roles.
- Add email generation and sending for full outreach automation.
- Use filters for location, company size, etc.

---

## Author
BY Pushpender 