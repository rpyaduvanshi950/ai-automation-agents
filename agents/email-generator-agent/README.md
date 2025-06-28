# ✉️ Email Generator Agent

## Overview
The Email Generator Agent is an AI-powered workflow for n8n that automates the process of generating and sending personalized cold outreach emails. It takes a plain-text prompt, extracts lead details, crafts a persuasive email using AI, and sends it via Gmail.

---

## Features
- Converts natural-language prompts into structured lead data (name, role, company, etc.)
- Uses advanced prompt engineering for high-conversion cold emails
- Sends emails automatically via Gmail
- Optional: Logs output to Google Sheets

---

## How It Works
1. **Trigger**: The workflow starts with a form or webhook trigger where you input a plain-text message (e.g., "Write a friendly email to Sarah, Product Manager at OpenAI about our AI writing tool.").
2. **Extract Lead Details**: An LLM node parses the message and extracts fields like name, role, company, product description, and tone.
3. **Prompt Generation**: Another node creates a tailored prompt for the AI to generate a cold email.
4. **Email Generation**: The AI (via OpenRouter or OpenAI) writes a persuasive email body and subject line.
5. **Send Email**: The workflow sends the generated email via Gmail (OAuth2 required).
6. **(Optional) Log to Google Sheets**: You can add a node to log sent emails and lead details.

---

## Required Credentials
- **Gmail**: OAuth2 credentials for sending emails
- **OpenRouter/OpenAI**: API key for LLM nodes
- *(Optional)* Google Sheets: OAuth2 credentials for logging

---

## Step-by-Step Setup
1. **Import the Workflow**: In n8n, import `Email_Generation_agent.json` from this folder.
2. **Configure Credentials**:
   - Set up Gmail OAuth2 in n8n and select it in the Gmail node.
   - Add your OpenRouter or OpenAI API key for the LLM nodes.
   - (Optional) Set up Google Sheets OAuth2 if logging.
3. **Trigger the Workflow**:
   - Use the included form or connect a webhook/chat trigger.
   - Enter a prompt describing the email you want to generate.
4. **Review & Send**:
   - The workflow will extract details, generate the email, and send it automatically.
   - Check your Gmail sent folder for results.
5. **(Optional) Logging**:
   - Add a Google Sheets node to log each sent email for tracking.

---

## Example Prompt
```
Write a concise, friendly outreach email to Jane Doe, Product Lead at AIFlow, about our automation product. Include a subject line. Signed, puspender.
```

---

## Tips & Customization
- Edit the prompt templates in the workflow for your brand voice.
- Add extra logic for follow-ups or A/B testing.
- Use with other n8n automations for full sales pipelines.

---

## Author
BY Pushpender 