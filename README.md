# Week 4 Starter: Math Agent

A ReAct agent that solves questions using tool calls.

## Demo Video
[Watch the Walkthrough] (https://docs.google.com/videos/d/19bkyIAAhZL6MX3Ktjenwd-zZBS2hRSjhGmRMzWkElsI/edit?usp=sharing)

## Setup

1. Install [uv](https://docs.astral.sh/uv/getting-started/installation/) if you don't have it.

2. Copy `.env.example` to `.env` and add your API key:
   ```bash
   cp .env.example .env
   ```
   Then edit `.env` and replace `your-key-here` with your key from [Google AI Studio](https://aistudio.google.com/apikey).

   To use a different provider, change the `MODEL` variable in `agent.py` and set the matching key in `.env`.

3. Make sure `.env` is in your `.gitignore` so you don't commit your key.

## Run

```bash
uv run agent.py
```

uv will install dependencies automatically on first run.

The agent will work through each question in `math_questions.md` and print the ReAct trace (Reason / Act / Result) for each one.

## Files

- `agent.py` - the ReAct agent (this is the file you'll modify)
- `calculator.py` - calculator tool
- `products.json` - product catalog with prices
- `math_questions.md` - the questions the agent solves
- `.env.example` - template for your API key
