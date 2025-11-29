# AI Content Curator & Publisher Workflow for n8n

This is an automated workflow for **n8n** that acts as a "Human-in-the-Loop" social media bot. It fetches news, drafts tweets using AI, and requests approval before posting.

## Features
- **Daily Trigger:** Runs automatically every day at 9:00 AM.
- **Content Sourcing:** Fetches articles from Google News RSS (Theme: AI & Machine Learning).
- **AI Processing:** Uses OpenAI (GPT-4.1-mini) to analyze relevance and draft tweets.
- **Human Approval:** Sends a draft to **Slack** with "Approve" and "Reject" buttons.
- **Publishing:** Automatically posts to **X (Twitter)** upon approval.

## Requirements
To run this workflow, you need n8n credentials for:
- OpenAI API
- Slack API
- Twitter/X API (OAuth2)

## How to use
1. Import the `.json` file into your n8n instance.
2. Update the credentials in the nodes.
3. Configure the "Workflow Configuration" node to change the search topic.
