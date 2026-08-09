# Stock Predictions AI

Web app that generates natural-language analysis of stock price movements
by fetching market data and passing it to an LLM for interpretation.

Built as the capstone project for Scrimba's "Build AI Apps with ChatGPT,
DALL·E and GPT-4" certification.

## What it does
- Takes one or more stock tickers as input
- Fetches historical price data from a market data API
- Sends the dataset to the OpenAI API with a prompt engineered to produce
  a concise, readable market report
- Renders the generated analysis in the UI

## Stack
JavaScript · Vite · OpenAI API · Polygon.io API

## Running locally
npm install
npm run dev

Requires an OpenAI API key and a market data API key in a .env file.
See .env.example.

## Notes
This was a learning project. The API key handling is client-side, which is
fine for a local demo but would need a backend proxy in production.
Happy Coding!
