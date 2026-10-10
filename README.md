# AI Telegram Support Bot - n8n + RAG

An intelligent Telegram support bot that answers user queries using a Google Docs Knowledge Base via RAG and logs all interactions.

## 🧠 System Architecture
![System Architecture](assets/workflow-diagram.png)

### How it Works
1.  **Trigger:** User sends a message on Telegram.
2.  **AI Agent + Knowledge Base:** The AI Agent retrieves relevant information from Google Docs using RAG/Tools and generates a contextual answer.
3.  **Actions:**
    *   **3A - Reply:** Sends the AI-generated response back to the user on Telegram.
    *   **3B - Log:** Records the full conversation (User Query, Bot Response, Timestamp) into Google Sheets for analytics.

## ⚙️ n8n Workflow Implementation
This is the actual n8n canvas implementation.
![n8n Workflow](assets/n8n-screenshot.png)

## 🎥 Live Demo
Watch the bot in action:
**[▶️ Watch Full Demo Video Here](https://your-loom-link-here)**

> Replace the link above with your Loom video link after recording.

## 🚀 Setup & Installation

1.  **Import Workflow:** Import `workflow.json` into your n8n instance.
2.  **Telegram:** Create a bot via @BotFather and add your Bot Token to the Telegram Trigger and Telegram Reply nodes.
3.  **Google Credentials:** Connect your Google Docs and Google Sheets credentials via OAuth2.
4.  **AI Model:** Connect your OpenAI / Gemini / Claude credentials to the AI Agent node.
5.  **Activate:** Activate the workflow and start chatting with your bot on Telegram.

## 📂 Repository Structure
-   `workflow.json` - The complete importable n8n workflow file
-   `assets/workflow-diagram.png` - High-level system architecture diagram
-   `assets/n8n-screenshot.png` - Screenshot of the built n8n workflow

## 🛠️ Tech Stack
-   n8n (Workflow Automation)
-   Telegram Bot API
-   OpenAI / LLM for AI Agent
-   Google Docs (Knowledge Base - RAG)
-   Google Sheets (Conversation Logging)

---
Built by [Maxwell Kelvin] - n8n Automation Builder
