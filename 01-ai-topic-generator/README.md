# AI Topic Generator

An AI-powered content ideation and LinkedIn content generation workflow built with n8n. It researches current Product Management and AI discussions, generates structured content topics, and processes each topic into a LinkedIn post draft before storing the results in Airtable.

## What It Does

This workflow:

1. Receives a topic or subject through an n8n form.
2. Uses an AI-powered Topic Finder to research recent Product Management and AI discussions.
3. Uses Google Gemini, Tavily, and Google search via SerpApi for research.
4. Generates exactly five structured LinkedIn discussion topics across different content categories.
5. Uses a Structured Output Parser to organize the generated topics.
6. Splits the topics into individual items.
7. Processes each topic through a Post Writer AI Agent.
8. Uses Groq to generate a LinkedIn post based on the selected topic and opening style.
9. Stores the generated topic, post draft, and completion status in Airtable.

## Workflow

Form Submission → Topic Finder → Split Out → Loop Over Items → Post Writer → Create Airtable Record

## Topic Finder

The Topic Finder researches recent Product Management and AI discussions and generates five structured LinkedIn content topics.

### Research & AI Components

- Google Gemini
- Tavily
- Google Search via SerpApi
- Structured Output Parser

### Topic Categories

The workflow generates one topic for each category:

1. Contrarian Opinion
2. Industry Trend
3. Product Failure Lesson
4. Customer Insight
5. Future Prediction

Each generated topic includes:

- Topic
- Opening style
- Category
- Content description

## Post Writer

The Post Writer AI Agent turns each generated topic into a LinkedIn post.

The workflow is designed to:

- Keep the post focused on the selected topic
- Use the specified opening style
- Avoid repetitive LinkedIn-style openings
- Provide practical product insights
- End with a discussion question
- Include 3–5 relevant hashtags
- Produce posts of approximately 200–250 words

## Key Concepts

- AI Agent orchestration
- AI-powered content ideation
- Prompt engineering
- LLM integration
- Web research
- Structured output generation
- Content generation
- Workflow automation
- Item looping and processing
- Airtable integration

## Tools & Technologies

- n8n
- Google Gemini
- Groq
- Tavily
- SerpApi
- Airtable
- AI Agents
- Structured Output Parser

## Runtime

This workflow was built and tested using a locally running n8n instance.

To execute the workflow, the required n8n environment and connected credentials must be configured locally.

## Project Purpose

This project demonstrates how AI agents, web research, structured outputs, and workflow orchestration can be combined to automate content ideation and accelerate a repeatable LinkedIn content creation workflow.
