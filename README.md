# ForexWise — Responsible Forex Education Assistant

A simple, beginner-friendly AI assistant that answers frequently asked questions
about **responsible forex education** and **getting started with forex trading**.

## What it does

- Answers beginner questions: what forex is, how to start, risk management,
  leverage dangers, broker safety, scam awareness, trading psychology, and more.
- **Safety-first by design**: never gives trade signals or financial advice;
  consistently emphasizes that most retail traders lose money.
- Curated knowledge base of 16 expert-reviewed FAQ topics — works fully offline.

## Two modes

| Mode | When | How it answers |
|---|---|---|
| **FAQ mode** (default) | Always available | Keyword-matched answers from the built-in knowledge base |
| **Live LLM mode** | When an OpenAI-compatible local server is running (e.g. LM Studio on port 1234) | Model-generated answers, grounded in the same knowledge base via a strict system prompt |

The header badge shows which mode is active. If the LLM call fails at any
moment, the app falls back to FAQ mode automatically.

## Run it

```powershell
python app.py
```

Then open **http://localhost:8000** in your browser.

- To enable **Live LLM mode**: start the LM Studio local server
  (Developer tab → Start Server, port 1234) with a model loaded, then
  refresh the page.

## Files

- `app.py` — HTTP server, FAQ knowledge base, LLM client, and embedded web UI
  (standard library only — no pip installs needed).

## Disclaimer

This tool is for **education only** and is **not financial advice**.
Forex trading carries a high risk of loss. Never trade with money you
cannot afford to lose.
