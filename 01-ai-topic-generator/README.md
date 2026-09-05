# AI Topic Generator

An AI-powered content ideation workflow built with n8n to discover relevant content topics and generate structured topic ideas for LinkedIn content planning.

## What It Does

This workflow:

1. Receives a content request through a form submission.
2. Uses an AI-powered Topic Finder to identify relevant content topics.
3. Uses Google Gemini to support topic generation.
4. Uses Tavily for web search and topic research.
5. Uses a Structured Output Parser to organize the generated topic data.
6. Splits the generated topics into individual items.
7. Processes the topics through a Post Writer AI Agent.
8. Uses a Groq-hosted language model to support post generation.
9. Creates a record in Airtable for the generated content.

## Workflow

Form Submission → Topic Finder → Split Out → Loop Over Items → Post Writer → Create Airtable Record

### Topic Finder

The Topic Finder combines AI generation, web search, and structured output to produce relevant content topics.

**Components:**
- Google Gemini Chat Model
- Tavily
- Structured Output Parser

### Post Writer

The Post Writer processes individual topics and generates content using an AI Agent.

**Components:**
- AI Agent
- Groq Chat Model
- Google Sheets

## Key Concepts

- AI Agent orchestration
- AI-powered content ideation
- Prompt engineering
- LLM integration
- Web research
- Structured output generation
- Workflow automation
- Data processing and item looping
- Airtable integration

## Tools & Technologies

- n8n
- Google Gemini
- Groq
- Tavily
- Airtable
- Google Sheets
- AI Agents
- Structured Output Parser

## Runtime

This workflow was built and tested using a locally running n8n instance.

To execute the workflow, the required n8n environment and connected credentials must be configured locally.

## Project Purpose

This project demonstrates how AI agents, web research, structured outputs, and workflow orchestration can be combined to automate content ideation and support a repeatable content creation process.
