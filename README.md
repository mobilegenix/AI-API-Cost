# 🧠 AI API Cost Simulation Dashboard

A React Native prototype to **simulate, visualize, and track** token usage and cost predictions for AI APIs like OpenAI or Anthropic. Built with developer velocity, observability, and budget-conscious deployments in mind.

---

## 🚀 Features

- 📊 Real-time cost estimation based on model, token size, and usage frequency
- 📈 Line charts visualizing weekly token consumption and API cost
- 🔌 Logging hook for Datadog/Grafana integration
- 📤 Export historical data as CSV or JSON
- ✅ Unit tests with Jest & React Native Testing Library
- 🔁 CI pipeline using GitHub Actions

---

## 🧱 Architecture

```plaintext
User Input (Tokens, Model, Requests)
        ↓
   Cost Simulator Engine (React State + Hook)
        ↓
  ┌──────────────┐     ┌────────────────────┐
  │ CSV / JSON   │ ←→  │ Visualization      │
  │ Export Utils │     │ (Recharts, Dual Y)│
  └──────────────┘     └────────────────────┘
        ↓
   Logging Hook
        ↓
  Observability Platform (Datadog, Grafana)
