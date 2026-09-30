# Signal: RAG-Based AI Content Feed

A full-stack app that delivers **personalized content** using Retrieval-Augmented Generation (RAG). A React front end talks to a Node.js/Express.js API (3 API endpoints), which calls a Python AI service that combines a vector database with the Gemini LLM through LangChain.

## Architecture

React (UI) → Node.js / Express.js (API layer) → Python AI service (vector database + Gemini via LangChain)

## How it works (retrieve-then-answer)

1. The user sends a request from the React interface.
2. The Express.js API forwards it to the Python AI service.
3. The AI service retrieves the most relevant items from the vector database.
4. Gemini (via LangChain) generates a personalized answer from that context.
5. The API parses the response and the UI renders the feed.

## Tech Stack

- **Front end:** React
- **API layer:** Node.js, Express.js
- **AI service:** Python, LangChain, Gemini LLM
- **Retrieval:** Vector database

## Getting Started

Add your steps here (install, run, and the Gemini API key in a `.env` file, never commit it).

## Challenges Solved

Debugged and fixed API response parsing across the front-end/back-end boundary in the retrieve-then-answer workflow.

## Author

Anusha Sinka: [GitHub](https://github.com/sinkaanusha367-art) | [LinkedIn](https://www.linkedin.com/in/anusha-sinka-4a3a192b8)

[Edit in StackBlitz](https://stackblitz.com/~/github.com/sinkaanusha367-art/signal-ai-feed)