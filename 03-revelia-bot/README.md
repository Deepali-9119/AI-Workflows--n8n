# ReveliaBot

An AI-powered Telegram assistant built with n8n that handles both text and image-based messages using Google Gemini.

## What It Does

ReveliaBot supports two types of user interactions:

1. Text messages
2. Image messages

The workflow automatically detects the message type and routes it to the appropriate AI processing path.

## Workflow

Telegram Trigger → If

### Text Message Flow

When the incoming Telegram message is a text message:

1. The message is passed to an AI Agent.
2. Google Gemini 2.5 Flash is used as the language model.
3. Conversation memory maintains context using the Telegram chat ID.
4. A Date & Time tool is available to the AI Agent.
5. The generated response is sent back to the user through Telegram.

**Flow:**

Telegram Trigger → If → AI Agent → Send a Text Message

### Image Message Flow

When the incoming Telegram message contains an image:

1. The workflow detects the image.
2. Google Gemini 2.5 Flash analyzes the image.
3. The image analysis is instructed to identify the main subject, important objects, and visible text.
4. The response is kept concise and returned to the user through Telegram.

**Flow:**

Telegram Trigger → If → Analyze an Image → Send a Text Message

## AI Agent

The AI Agent acts as the conversational assistant for text-based interactions.

It is instructed to:

- Respond in a conversational tone
- Keep answers short and useful
- Respond naturally to greetings
- Give direct answers to general questions
- Provide a concise summary before details for complex topics
- Use bullet points when appropriate
- Avoid long paragraphs
- Keep most responses under 100 words

## Image Analysis

The image-processing branch uses Google Gemini to analyze incoming images.

The image assistant is instructed to:

- Describe the image naturally
- Identify the main subject
- Mention important objects
- Mention visible text when present
- Keep the response under 100 words
- Avoid unnecessary detail

## Memory

The workflow uses Simple Memory to maintain conversational context.

The Telegram chat ID is used as the session key, allowing conversations to maintain separate memory across users or chats.

## Tools & Technologies

- n8n
- Telegram
- AI Agents
- Google Gemini
- Search API
- Simple Memory
- Date & Time Tool
- Prompt Engineering
- Workflow Automation

## Workflow Architecture

The workflow follows a message-routing architecture:

**Input:** Telegram message

**Routing:** If node determines whether the message contains an image

**Text Processing:** AI Agent + Google Gemini + Memory + Date & Time

**Image Processing:** Google Gemini image analysis

**Output:** Telegram response

## Key Concepts

- AI Agent orchestration
- Multimodal AI interaction
- Image analysis
- Conversational memory
- Telegram bot integration
- Conditional workflow routing
- LLM integration
- Tool-enabled AI agents
- Prompt engineering
- Workflow automation

## Runtime

This workflow was built and tested using a locally running n8n instance.

To execute the workflow, the required n8n environment and connected credentials must be configured locally.

## Project Purpose

This project demonstrates how n8n can be used to build a practical AI assistant that combines conversational AI, image understanding, memory, external tools, and Telegram-based interaction in a single workflow.
