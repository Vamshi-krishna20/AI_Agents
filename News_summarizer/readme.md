# AI News Summarizer - n8n Workflow

This repository contains an automated n8n workflow that fetches AI-related news from RSS feeds, summarizes them using Google Gemini, and sends a daily email report via Gmail.

## 🚀 Workflow Overview

The workflow performs the following steps:

1.  **Schedule Trigger**: Runs daily at 10:00 AM.
2.  **RSS Read**: Fetches the latest news from `aibusiness.com`.
3.  **Aggregate**: Combines all news items for processing.
4.  **Google Gemini (LLM)**: Summarizes the articles and formats them into a professional email body.
5.  **Gmail Node**: Sends the summary to the specified recipient.

## 🛠️ How to Use

1.  **Import to n8n**:
    - Download the `ai_news_summarizer_workflow.json` file.
    - In your n8n instance, go to "Workflows" -> "Import from File".
2.  **Configure Credentials**:
    - Set up your **Google Gemini (PaLM)** API credentials.
    - Connect your **Gmail** account using OAuth2.
3.  **Customize Email**:
    - Edit the `Send a message` node to update the recipient's email address.

## 📦 Requirements

- [n8n](https://n8n.io/) (Self-hosted or Cloud)
- Google Gemini API Key
- Gmail Account (for sending emails)

---

_Created with 🧠 AI-assisted automation._
