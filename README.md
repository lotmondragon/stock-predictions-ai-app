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

No API keys are needed locally: both external calls go through Cloudflare
Workers that hold the OpenAI and Polygon.io keys server-side.

## Notes
This was a learning project. API keys never reach the browser: the frontend
calls two Cloudflare Workers that act as a proxy to OpenAI and Polygon.io.
A production version would add rate limiting and input validation on the
Workers.
