### Hi, I'm Vamsi Alla 👋

**Senior Software Engineer** · Building production AI systems (LLM, RAG, agents)

12+ years building production software and 3+ years designing, evaluating and deploying LLM and agentic AI applications. I work directly with customers to find the real problem, then own the solution from architecture to evaluation, deployment and handoff.

Open to Forward Deployed Engineer and senior AI engineering roles · Remote, USA

🌐 [Portfolio](https://vamsialla.com) · 💼 [LinkedIn](https://www.linkedin.com/in/vamsi-alla/) · ✉️ vamsialla.dev@gmail.com

---

#### 📏 New: [Eval Harness](https://github.com/vamsialladev/eval-harness)

<a href="https://vamsialla.com/projects/eval-harness.html#demo"><img src="https://raw.githubusercontent.com/vamsialladev/eval-harness/main/docs/images/demo.gif" alt="The live Eval Harness dashboard: the regression demo run filtered to failing cases, and question q13 drilled down to its expected passage, three refused answers and failed verdicts" width="640"></a>

**[▶ Watch the demo (with narration)](https://vamsialla.com/projects/eval-harness.html#demo)** · **[Open the live dashboard](https://eval-harness.streamlit.app)** (read-only, no API calls)

Stage 3 of the same simulated hotel engagement. One evaluation system for both assistants below: one case schema, each project's own metrics, honest intervals and regression gates in both repos' CI, so a prompt, model or retrieval change can't lower quality without a red check.

- **Caught a real regression:** a "send 2 passages instead of 5" change kept retrieval inside its confidence interval (98% → 93%), but the gate failed because q13 and q35 always passed and now always failed
- **Judge calibrated honestly:** an LLM judge agreed with my first 40 hand labels 95% of the time with Cohen's kappa **0.00** (no failures in them); a second blind round built to contain failures reached **0.29**, so no judge score is trusted or gated
- **Reproduces published numbers:** the harness re-scores both projects' recordings to their exact published results, and fresh re-runs at pinned commits pass every gate
- **Production habits:** 181 labelled cases, 87 tests, 93% coverage, every saved report re-scored in CI, 21 recorded decisions, **$0.41** total API spend

[Live dashboard](https://eval-harness.streamlit.app) · [Demo video](https://vamsialla.com/projects/eval-harness.html#demo) · [Case study](https://vamsialla.com/projects/eval-harness.html) · [Code](https://github.com/vamsialladev/eval-harness)

#### ✉️ Featured: [Guest Request Agent](https://github.com/vamsialladev/guest-request-agent)

<a href="https://vamsialla.com/projects/guest-request-agent.html#demo"><img src="https://vamsialla.com/assets/img/guest-agent-still.jpg" alt="The live Guest Request Agent's step timeline for a guest email: booking found, three hotel policies searched and cited, two staff tasks proposed, checks passed" width="640"></a>

**[▶ Watch the 2-minute demo (with narration)](https://vamsialla.com/projects/guest-request-agent.html#demo)** · **[Try the live app](https://guest-request-agent.streamlit.app)** (no sign-in, nothing is ever sent)

Stage 2 of the same simulated hotel engagement, with synthetic guests and bookings. An agent reads a guest email, finds every request, checks the guest's own booking, free rooms and hotel policy (using stage 1's search as a tool), drafts a cited reply and proposes tasks. Staff approve, edit or reject every draft; refunds, upgrades and changes are only ever proposed to a manager.

- **Gated in CI:** 100% escalation recall, 100% prompt-injection resistance and zero forbidden promises over 40 labelled emails × 3 runs, plus 100% on a held-out set; **$1.30 per 1,000 emails**, 8.4 s p95
- **Measured honestly:** eight gate failures were bugs in my own checks, each fixed with a regression test; the escalation rules missed both held-out escalations and the model caught them
- **Built to be safe by construction:** tools can only read or propose, the booking lookup is scoped to the sender, every fact is checked against tool results
- **Production habits:** 237 tests, 98% coverage, recorded eval runs re-scored in CI, owner admin page with a full request log, 17 recorded decisions

[Live demo](https://guest-request-agent.streamlit.app) · [2-minute video](https://vamsialla.com/projects/guest-request-agent.html#demo) · [Case study](https://vamsialla.com/projects/guest-request-agent.html) · [Code](https://github.com/vamsialladev/guest-request-agent)

#### 🛎️ Featured: [Hotel Operations Knowledge Assistant](https://github.com/vamsialladev/hotel-ops-assistant)

<a href="https://vamsialla.com/projects/hotel-ops-assistant.html#demo"><img src="https://raw.githubusercontent.com/vamsialladev/hotel-ops-assistant/main/docs/images/demo.gif" alt="The live Hotel Operations Knowledge Assistant: a front-desk agent clicks a suggested question about dogs at Beach Resort and a cited answer streams in with its source" width="640"></a>

**[▶ Watch the 2-minute demo (with narration)](https://vamsialla.com/projects/hotel-ops-assistant.html#demo)** · **[Try the live app](https://hotel-ops-assistant.streamlit.app)** (no sign-in)

A simulated client engagement with synthetic hotel documents. Front-desk staff ask policy questions in plain English and get short, streamed answers with the source for every fact, for the right hotel. It refuses when the documents don't say, corrects wrong facts in the question, and points to a manager for refunds and safety.

- **Measured, not guessed:** 54-question eval (prompt injection, must-refuse, wrong facts, off-topic, escalation), 3 runs: **97–98% answer accuracy**, full answer p95 about 2.5 s, **$0.17 per 1,000 questions**; the first question a visitor types gets a useful result **100%** of the time (43% before I tested it that way)
- **Debugged with evidence:** the eval caught my own grader passing a wrong answer; a "$75 fee" bug traced to a number in the question; model choice (Claude Haiku 5.5 over 4.5) made by measurement
- **Product, not a notebook:** in-app guidance, curated follow-ups and "Did you mean" recovery, Insights for managers, a document library, light/dark mode, phone layout and public-demo protections
- **Production habits:** 307 tests, 97% coverage, CI with a dependency audit and eval gates, Docker, threat model, 50 recorded decisions
- **Business case:** projected value with pessimistic, base and optimistic scenarios (about $32K/yr base for 2 hotels), plus a pilot plan with go / no-go KPIs

[Live demo](https://hotel-ops-assistant.streamlit.app) · [2-minute video](https://vamsialla.com/projects/hotel-ops-assistant.html#demo) · [Case study](https://vamsialla.com/projects/hotel-ops-assistant.html) · [Code](https://github.com/vamsialladev/hotel-ops-assistant)

#### 🔨 In progress
**Production Deployment** (stage 4 of 5): run history, monitoring, sign-in and personal-data redaction for the assistants.

#### 🧰 Tools I work with
Python · Claude API (tool use) · Pydantic · RAG (BM25 + embeddings) · Evaluation (LLM-as-judge, Cohen's kappa, Wilson intervals) · Streamlit · pytest · Playwright · GitHub Actions · Docker

#### 🧭 How I work
**Understand** the problem and what it costs → **build** with the data as it really is → **measure** with evals → **deploy** under real limits → **hand off** with docs the team can own.
