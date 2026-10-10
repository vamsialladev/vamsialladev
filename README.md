### Hi, I'm Vamsi Alla 👋

I build AI systems for **hospitality operations**, and I take them from the business problem to a deployed, measured, documented system. I'm working toward **Forward Deployed Engineer** roles: working directly with customers to turn messy, real-world problems into AI that works.

🌐 [Portfolio](https://vamsialladev.github.io) · 💼 [LinkedIn](https://www.linkedin.com/in/vamsi-alla/) · ✉️ vamsialla.dev@gmail.com

---

#### 🛎️ Featured: [Hotel Operations Knowledge Assistant](https://github.com/vamsialladev/hotel-ops-assistant)
Front-desk staff ask policy questions in plain English and get short, streamed answers with the source for every fact, for the right hotel. It refuses when the documents don't say, corrects wrong facts in the question, and points to a manager for refunds and safety.

- **Measured, not guessed:** 54-question eval (prompt injection, must-refuse, wrong facts, off-topic, escalation), 3 runs: **96–98% answer accuracy**, full answer p95 about 2.5 s, **$0.17 per 1,000 questions**
- **Debugged with evidence:** the eval caught my own grader passing a wrong answer; a "$75 fee" bug traced to a number in the question; model choice (Claude Haiku 5.5 over 4.5) made by measurement
- **Product, not a notebook:** multi-page Streamlit app with Insights for managers, a document library, light/dark mode, phone layout and public-demo protections
- **Production habits:** 184 unit tests, 96% coverage, CI with a dependency audit, Docker, threat model, 33 recorded decisions
- **Business case:** projected value with pessimistic, base and optimistic scenarios (about $32K/yr base for 2 hotels), plus a pilot plan with go / no-go KPIs

[Live demo](https://hotel-ops-assistant.streamlit.app) · [Case study](https://vamsialladev.github.io/projects/hotel-ops-assistant.html) · [Code](https://github.com/vamsialladev/hotel-ops-assistant)

#### 🔨 In progress
**Guest Request Agent:** reads guest emails, checks bookings and policy, drafts replies, and waits for staff approval before anything is sent.

#### 🧰 Tools I work with
Python · Claude API · RAG (BM25 + embeddings) · Evaluation · Streamlit · pytest · Playwright · GitHub Actions · Docker

#### 🧭 How I work
**Understand** the problem and what it costs → **build** with the data as it really is → **measure** with evals → **deploy** under real limits → **hand off** with docs the team can own.
