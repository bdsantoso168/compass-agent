# 🧭 Compass -- AI-Powered Research & Analytics Agent
<p align="center">
  <img src=<img width="2048" height="2048" alt="compass-logo" src="https://github.com/user-attachments/assets/0afe86d5-0f29-4c19-b7d1-7d785b6b8d81" />
 alt="Compass Agent" width="200">
</p>

> **Navigate any research question with AI.**

Compass is an autonomous AI agent that answers business, research, and analytics questions by fetching **real data** from live sources -- not by guessing. Built with Claude (Anthropic) as the reasoning engine, it chains multiple tools together in multi-step workflows and remembers your full conversation context.

## Architecture

```
LLM (Claude Sonnet 4) + Tools (4 Real APIs) + Reasoning Loop + Memory = Compass
```

### The Agent Equation
| Component | Implementation |
|-----------|---------------|
| **Brain** | Claude Sonnet 4 -- decides which tools to use and when |
| **Tools** | 4 real API connections (Wikipedia, Web Fetcher, Calculator, News) |
| **Reasoning Loop** | Multi-step tool chaining with up to 8 iterations |
| **Memory** | Conversation history list passed to every Claude call |

## Tools

| Tool | Description | Data Source |
|------|-------------|-------------|
| wikipedia_search | Look up any company, person, or topic | Wikipedia REST API |
| web_fetcher | Extract text from any public webpage | requests + BeautifulSoup |
| calculator | Evaluate math expressions safely | Sandboxed Python eval |
| news_search | Pull latest headlines on any topic | Google News RSS |

## Quick Start

1. Open Compass_AI_Agent.ipynb in Google Colab
2. Get an Anthropic API key at console.anthropic.com
3. Paste your key in Cell 2
4. Run all cells

## Tech Stack

- **LLM:** Claude Sonnet 4 (Anthropic API)
- **Tools:** Wikipedia REST API, BeautifulSoup, Google News RSS, Python math
- **Environment:** Google Colab
- **Course:** ISOM 260/900 -- AI for Business, Suffolk University

## Author

**Benedict Daxell Santoso**
- Business Analytics & Information Systems, Suffolk University (May 2026)
- LinkedIn: linkedin.com/in/benedictdaxellsantoso
- GitHub: github.com/bdsantoso168
