# 🤖 AI Workflows — n8n Automation Suite

**A collection of AI-powered automation workflows built with n8n, exploring how LLMs, APIs, and workflow orchestration can be combined to automate practical tasks.**

*n8n · AI Agents · Prompt Engineering · Workflow Automation*

[![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white)](https://n8n.io/)
[![Google Gemini](https://img.shields.io/badge/Google_Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)](https://gemini.google.com/)
[![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square)](https://groq.com/)

---

## 📌 Why This Exists

As an aspiring Product Manager focused on AI products, I want to understand how AI-powered experiences work beyond the user interface — including orchestration, routing, integrations, and automation.

These workflows represent hands-on exploration of:

- **AI orchestration**: Connecting AI models and tools into structured workflows
- **Prompt engineering**: Designing prompts for different AI use cases
- **API integration**: Connecting search, data, messaging, and webhook-based services
- **Automation thinking**: Identifying repetitive processes that can benefit from AI-powered automation

---

## 🔧 Workflows

### 01. AI Topic Generator

**Purpose**: AI-powered content ideation and LinkedIn post generation focused on Product Management and AI topics.

| Component | Tool |
|-----------|------|
| Research | Tavily, SerpApi |
| Generation | Google Gemini, Groq |
| Output | Structured topic briefs + LinkedIn post drafts |
| Storage | Airtable |

**How it works**:

1. Researches current Product Management and AI discussions
2. Generates structured content topics with AI
3. Produces LinkedIn post drafts
4. Saves the generated content to Airtable for tracking

**Product Insight**: This workflow explores how AI can automate a personal content workflow from research and ideation through drafting and organization.

[View Workflow Details →](./01-ai-topic-generator)

---

### 02. Rumi's Muse

**Purpose**: An AI poetry workflow that transforms a user-provided topic or situation into a Rumi-inspired reflective poem.

| Component | Tool |
|-----------|------|
| AI Agent | Google Gemini |
| Integration | Webhook → n8n → AI response |

**How it works**:

1. User submits a topic or situation through the web prototype
2. A webhook sends the request to the n8n workflow
3. The AI Agent generates a Rumi-inspired poem
4. The response is returned to the frontend

**Product Insight**: This project explores how a simple user experience can connect to an AI workflow through webhooks while keeping the underlying orchestration invisible to the user.

[View Workflow Details →](./02-rumis-muse)

---

### 03. ReveliaBot

**Purpose**: A multimodal Telegram AI assistant that handles both text and image messages.

| Component | Tool |
|-----------|------|
| AI Model | Google Gemini |
| Platform | Telegram Bot API |
| Memory | Conversational memory |
| Routing | Conditional workflow routing |

**How it works**:

1. User sends a text or image message to the Telegram bot
2. The workflow detects the message type
3. The request is routed to the appropriate processing branch
4. Gemini processes the input with conversational context
5. The response is sent back to the user in Telegram

**Product Insight**: Building a multimodal AI experience requires different processing paths for different input types while keeping the overall interaction simple for the user.

[View Workflow Details →](./03-revelia-bot)

---

## 🛠️ Tools & Technologies

| Category | Tools |
|----------|-------|
| Workflow Platform | n8n |
| AI Models | Google Gemini, Groq |
| Search & Research | Tavily, SerpApi |
| Data Storage | Airtable |
| Messaging | Telegram Bot API |
| Integration | Webhooks, API integrations |
| Core Skills | Prompt Engineering, Workflow Automation, AI Orchestration |

---

## 📝 What I Learned

- **AI orchestration as a product skill**: Understanding how AI models, tools, data sources, and integrations can be connected into useful workflows
- **Prompt engineering matters**: Prompt structure and constraints can significantly affect AI outputs, making iteration important
- **Workflow thinking**: Breaking a process into modular steps helps identify opportunities for automation and clearer system design
- **Multimodal AI experiences**: Supporting text and image inputs requires different processing paths while maintaining a consistent user experience

---

*Built by [Deepali Shah](https://github.com/Deepali-9119) · Aspiring Product Manager | AI Product Builder*
