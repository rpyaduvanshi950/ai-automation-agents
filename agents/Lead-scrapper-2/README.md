# 🕵️‍♂️ Lead Scrapper 2 – Advanced Lead Generation Suite

## Overview
The `Lead-scrapper-2` folder contains a powerful set of n8n workflows and tools for advanced lead generation, enrichment, and research. It leverages multiple APIs (Apollo.io, Relevance AI, Perplexity, TrustPilot) to scrape, research, and enrich leads, and features a conversational agent for guided lead collection.

---

## Key Workflows & Tools

- **Lead_Scraping___2_0 (1).json**  
  Scrapes leads from Apollo.io via Apify API, extracting detailed info (name, email, phone, company, job title, seniority, LinkedIn URL, etc.) and saves to Google Sheets. Designed for high-volume, structured scraping.

- **Lead_Scraping.json**  
  Similar to the above, with possible variations in API keys or sheet destinations.

- **Lead_Research.json**  
  Enriches leads by researching their LinkedIn profiles, recent posts, and company info. Integrates with Relevance AI and Perplexity for deep research, and fetches TrustPilot reviews for company reputation.

- **Lead_Gen_Joe.json**  
  Implements a conversational agent ("Lead Generation Joe") that interacts with users, asks clarifying questions, and triggers scraping or research workflows based on user input. Supports structured queries for location, business, and job title.

- **Relevance AI LinkedIn Scraper Tool.rai**  
  Configuration or script for Relevance AI's LinkedIn scraping capabilities.

- **Excel Template.xlsx**  
  Template for storing or importing/exporting lead data.

- **Webhook cURL Request.docx**  
  Example/documentation for triggering workflows via webhook/cURL.

---

## Capabilities
- **Multi-Source Scraping:** Apollo.io (via Apify) and Relevance AI for robust LinkedIn and company data extraction.
- **Lead Enrichment:** Researches company background, recent posts, and reviews using Perplexity and TrustPilot.
- **Conversational Agent:** "Lead Generation Joe" guides users through the process, ensuring all required info is collected before scraping or research.
- **Flexible Output:** Data is saved to Google Sheets or Excel, ready for further processing or outreach.
- **API-Driven:** Workflows are triggered via n8n, webhooks, or other workflows, and use API keys for authentication.

---

## Setup & Usage

1. **Import the desired workflow(s) into n8n.**
2. **Configure API keys** for Apify (Apollo.io), Relevance AI, Perplexity, TrustPilot, and Google Sheets as needed.
3. **Use the conversational agent** (Lead_Gen_Joe) for guided scraping, or trigger scraping/research workflows directly.
4. **Review and use the output** in Google Sheets or Excel.

### Example Use Cases
- Scrape hundreds of leads from LinkedIn with emails, phones, and company info.
- Research a lead's company, recent activity, and reputation before outreach.
- Use a chat interface to specify exactly what leads you want, and let the agent handle the rest.

---

## Example Workflow: Lead Generation Joe
- Start a conversation with Lead Generation Joe.
- Specify locations, business types, and job titles.
- The agent will ask clarifying questions if needed.
- Once all info is collected, the agent triggers the scraping workflow and notifies you when leads are added to the sheet.
- You can then request research on specific leads by providing their LinkedIn URLs.

---

## Author
BY Pushpender 