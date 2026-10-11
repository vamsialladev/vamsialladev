### Hi, I'm Vamsi Alla 👋

I build AI systems for **hospitality operations**, and I take them from the business problem to a deployed, measured, documented system. I'm working toward **Forward Deployed Engineer** roles: working directly with customers to turn messy, real-world problems into AI that works.

🌐 [Portfolio](https://vamsialla.com) · 💼 [LinkedIn](https://www.linkedin.com/in/vamsi-alla/) · ✉️ vamsialla.dev@gmail.com

---

#### 🛎️ Featured: [Hotel Operations Knowledge Assistant](https://github.com/vamsialladev/hotel-ops-assistant)

<a href="https://vamsialla.com/projects/hotel-ops-assistant.html#demo"><img src="https://raw.githubusercontent.com/vamsialladev/hotel-ops-assistant/main/docs/images/demo.gif" alt="The live Hotel Operations Knowledge Assistant: a front-desk agent clicks a suggested question about dogs at Beach Resort and a cited answer streams in with its source" width="640"></a>

**[▶ Watch the 2-minute demo (with narration)](https://vamsialla.com/projects/hotel-ops-assistant.html#demo)** · **[Try the live app](https://hotel-ops-assistant.streamlit.app)** (no sign-in)

A simulated client engagement with synthetic hotel documents. Front-desk staff ask policy questions in plain English and get short, streamed answers with the source for every fact, for the right hotel. It refuses when the documents don't say, corrects wrong facts in the question, and points to a manager for refunds and safety.

- **Measured, not guessed:** 54-question eval (prompt injection, must-refuse, wrong facts, off-topic, escalation), 3 runs: **97–98% answer accuracy**, full answer p95 about 2.5 s, **$0.17 per 1,000 questions**; the first question a visitor types gets a useful result **100%** of the time (43% before I tested it that way)
- **Debugged with evidence:** the eval caught my own grader passing a wrong answer; a "$75 fee" bug traced to a number in the question; model choice (Claude Haiku 5.5 over 4.5) made by measurement
- **Product, not a notebook:** in-app guidance, curated follow-ups and "Did you mean" recovery, Insights for managers, a document library, light/dark mode, phone layout and public-demo protections
- **Production habits:** 274 tests, 97% coverage, CI with a dependency audit and eval gates, Docker, threat model, 49 recorded decisions
- **Business case:** projected value with pessimistic, base and optimistic scenarios (about $32K/yr base for 2 hotels), plus a pilot plan with go / no-go KPIs

[Live demo](https://hotel-ops-assistant.streamlit.app) · [2-minute video](https://vamsialla.com/projects/hotel-ops-assistant.html#demo) · [Case study](https://vamsialla.com/projects/hotel-ops-assistant.html) · [Code](https://github.com/vamsialladev/hotel-ops-assistant)

#### 🔨 In progress
**Guest Request Agent:** reads guest emails, checks bookings and policy, drafts replies, and waits for staff approval before anything is sent.

#### 🧰 Tools I work with
Python · Claude API · RAG (BM25 + embeddings) · Evaluation · Streamlit · pytest · Playwright · GitHub Actions · Docker

#### 🧭 How I work
**Understand** the problem and what it costs → **build** with the data as it really is → **measure** with evals → **deploy** under real limits → **hand off** with docs the team can own.
