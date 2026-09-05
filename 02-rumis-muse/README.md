# Rumi's Muse

An AI-powered poetry assistant built with n8n that transforms a user-provided topic into a short, reflective poem through an AI Agent powered by Google Gemini.

## What It Does

This workflow:

1. Receives a topic through an HTTP POST webhook.
2. Passes the topic to an AI Agent.
3. Uses Google Gemini 3.1 Flash Lite as the language model.
4. Generates an 8–14 line poetic response.
5. Returns the generated poem through a webhook response.

## Workflow

Webhook → AI Agent → Respond to Webhook

### AI Agent

The AI Agent receives the user's topic and generates a poetic response based on predefined instructions.

The workflow is designed to produce:

- 8–14 lines
- Warm, spiritual, and reflective tone
- Poem text only
- No title
- No quotation marks
- No explanation of the poem

### Language Model

The AI Agent is connected to:

- Google Gemini 3.1 Flash Lite

## Key Concepts

- AI Agent orchestration
- Prompt engineering
- LLM integration
- Webhook-based interaction
- AI-generated creative content
- API-style workflow design
- Automated response generation

## Tools & Technologies

- n8n
- Google Gemini
- AI Agent
- Webhooks

## Workflow Architecture

The workflow uses a simple request → generation → response pattern:

**Input:** User-provided topic  
**Processing:** AI Agent + Google Gemini  
**Output:** Generated poem

## Runtime

This workflow was built and tested using a locally running n8n instance.

To execute the workflow, the required n8n environment and connected credentials must be configured locally.

## Project Purpose

This project demonstrates how an AI Agent, prompt engineering, and webhook-based workflow orchestration can be combined to create a simple AI-powered creative application.
