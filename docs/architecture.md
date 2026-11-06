# Architecture

| Component | Role | Status |
|---|---|---|
| Scheduler | Triggers Workflow A (Mon/Wed/Fri 10:00) and B (Mon 09:00) | Specified |
| Trend research | Web search on AI product design, AI tools, AI careers | Specified; provider unverified |
| ContentPost store | Holds post history, URN, status | Specified; storage unverified |
| Content generator | Writes the post in the owner's voice | Specified |
| Image generator | Creates the accompanying image | Specified; provider unverified |
| LinkedIn publisher | Posts content and image | Specified |
| Comment responder | Replies to unanswered comments | Specified; extent of automation unverified |
| Notifier | Sends hook, reasoning, link to owner | Specified; channel unverified |
| Analytics and reporting | Weekly engagement report | Specified; delivery channel unverified |

Diagrams: [`../architecture/system-architecture.mmd`](../architecture/system-architecture.mmd), [`../architecture/workflow-diagram.mmd`](../architecture/workflow-diagram.mmd), [`../architecture/weekly-report-diagram.mmd`](../architecture/weekly-report-diagram.mmd)
