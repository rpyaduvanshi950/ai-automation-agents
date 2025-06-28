# 📈 Stock Market Insights AI Agent

## Overview
The Stock Market Insights AI Agent is an n8n workflow that provides real-time stock market insights, news, and analysis for Indian stocks. It extracts the stock ticker from user input, fetches price data and news, and generates a professional summary and recommendation using AI.

---

## Features
- Extracts NSE stock ticker from user messages
- Fetches real-time price data from Yahoo Finance
- Retrieves latest news headlines for the company
- Uses AI to summarize market status, news sentiment, technical signals, and provide actionable insights

---

## How It Works
1. **Trigger**: The workflow starts with a chat or webhook trigger where you input a stock-related query (e.g., "What's the outlook for TCS?").
2. **Extract Ticker**: An LLM node parses your message to extract the correct NSE ticker symbol.
3. **Fetch Stock Data**: The workflow queries Yahoo Finance for the latest price, volume, and technical data.
4. **Fetch News**: It retrieves the latest news headlines about the company using NewsAPI.
5. **Summarize & Analyze**: An AI node generates a structured report covering market status, news sentiment, technical signals, and recommendations.

---

## Required Credentials
- **Yahoo Finance**: No API key required (public endpoint)
- **NewsAPI**: API key for fetching news headlines
- **OpenRouter/OpenAI/Ollama**: API key for LLM nodes (for analysis and summarization)

---

## Step-by-Step Setup
1. **Import the Workflow**: In n8n, import `Stock_Market_Insights_AI_Agent (1).json` from this folder.
2. **Configure Credentials**:
   - Add your NewsAPI key as an HTTP credential in n8n.
   - Add your OpenRouter, OpenAI, or Ollama API key for the LLM nodes.
3. **Trigger the Workflow**:
   - Use the chat/webhook trigger or run manually.
   - Enter a stock-related prompt (see below).
4. **Review Results**:
   - The workflow will output a detailed summary and recommendation for the stock.

---

## Example Prompts
```
What's the outlook for RELIANCE?
Show me the latest news and analysis for INFY.
Summarize the technicals and news for TCS.
```

---

## Tips & Customization
- Add more data sources or technical indicators as needed.
- Adjust the AI prompt for different analysis styles.
- Integrate with alerting or reporting workflows in n8n.

---

## Author
BY Pushpender 