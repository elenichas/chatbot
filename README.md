# AI Chatbot Sample

A small Express application that serves a browser chat interface and sends user messages to the OpenAI Chat Completions API.

## What it includes

- Static browser interface served by Express
- JSON endpoint for chatbot requests
- Server-side use of the `OPENAI_API_KEY` environment variable
- Conversation-message formatting for the OpenAI API

## Requirements

- Node.js 18 or later
- An OpenAI API key

## Run locally

```bash
git clone https://github.com/elenichas/chatbot.git
cd chatbot
npm install
export OPENAI_API_KEY="your-api-key"
npm start
```

Open `http://localhost:3000`.

Never commit API keys or place them in browser-side JavaScript. Use an environment variable or a secrets manager in deployed environments.

## Current scope

This is a learning prototype rather than a production chat service. Before production use, add request validation, authentication, rate limiting, structured error handling, moderation appropriate to the use case, and an actively supported model/API integration.

## Security

TLS certificate verification must remain enabled. If a development environment reports a certificate error, fix the local certificate chain rather than disabling verification globally.