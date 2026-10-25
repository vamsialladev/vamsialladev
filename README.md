### Hi, I'm Vamsi Alla 👋

**Senior Software Engineer** · Building production AI systems (LLM, RAG, agents)

I've built production software for 12+ years, and for the last 3+ I've been designing, evaluating and deploying LLM
and agentic AI applications for enterprise clients. What I like most is the part before the code: sitting with the
people who'll use the thing, finding the real problem, and then owning it all the way to a handoff their team can
run. I measure before I claim.

Open to Forward Deployed Engineer and senior AI engineering roles · Remote, USA

🌐 [vamsialla.com](https://vamsialla.com) · 💼 [LinkedIn](https://www.linkedin.com/in/vamsi-alla/) · ✉️ vamsialla.dev@gmail.com

---

#### 🧭 One engagement, end to end

My public projects are the stages of one simulated client engagement for a fictional hotel group (a beach resort
and a mountain lodge, all synthetic data), in the order I'd run it for a real client:

| Stage | What it is | Links |
|---|---|---|
| Pre-sales | **Account Research agent**: a cited discovery-prep brief before the first meeting | [Code](https://github.com/vamsialladev/fde-account-research-agent) |
| 0 | **Discovery & scoping**: six stakeholder sessions, a four-check test, SOW, pricing | [Case study](https://vamsialla.com/projects/hotel-ai-discovery.html) · [Pack](https://github.com/vamsialladev/hotel-ai-discovery) |
| 1 | **Knowledge Assistant**: cited policy answers for front-desk staff | [Live](https://hotel-ops-assistant.streamlit.app) · [Case study](https://vamsialla.com/projects/hotel-ops-assistant.html) · [Code](https://github.com/vamsialladev/hotel-ops-assistant) |
| 2 | **Guest Request Agent**: reads guest emails, drafts cited replies, staff approve | [Live](https://guest-request-agent.streamlit.app) · [Case study](https://vamsialla.com/projects/guest-request-agent.html) · [Code](https://github.com/vamsialladev/guest-request-agent) |
| 3 | **Eval Harness**: one regression gate for both assistants | [Live](https://eval-harness.streamlit.app) · [Case study](https://vamsialla.com/projects/eval-harness.html) · [Code](https://github.com/vamsialladev/eval-harness) |
| 4–5 | **Production & handoff**: eval-found fixes, redacted logs, kill switch, runbooks, SLOs | [Case study](https://vamsialla.com/projects/production-and-handoff.html) · [Handoff](https://github.com/vamsialladev/hotel-ai-handoff) |
| 6 | **Resort Activities Concierge**: guests ask, the agent requests bookings, staff approve | [Code](https://github.com/vamsialladev/resort-activities-concierge) |
| 7 | **MCP Tools + RBAC**: the group's tools for any MCP client, roles and an audit log | [Case study](https://vamsialla.com/projects/hotel-tools-mcp.html) · [Code](https://github.com/vamsialladev/hotel-tools-mcp) |
| 8 | **Ops Analytics**: plain-English questions over bookings, SQL always shown, daily anomaly check | [Case study](https://vamsialla.com/projects/hotel-ops-analytics-agent.html) · [Code](https://github.com/vamsialladev/hotel-ops-analytics-agent) |

---

#### 🛎️ [Hotel Operations Knowledge Assistant](https://github.com/vamsialladev/hotel-ops-assistant) (stage 1)

<a href="https://vamsialla.com/projects/hotel-ops-assistant.html#demo"><img src="https://raw.githubusercontent.com/vamsialladev/hotel-ops-assistant/main/docs/images/demo.gif" alt="The live Hotel Operations Knowledge Assistant: a front-desk agent asks about dogs at Beach Resort and a cited answer streams in with its source" width="640"></a>

**[▶ Watch the demo](https://vamsialla.com/projects/hotel-ops-assistant.html#demo)** (AI-narrated) · **[Try the live app](https://hotel-ops-assistant.streamlit.app)** (no sign-in)

Front-desk staff ask policy questions in plain English and get a short answer with the source for every fact, for
the right hotel. It refuses when the documents don't say. **100% answer accuracy** on a 54-question eval at **$0.18
per 1,000 questions**; testing like a first-time visitor took first-question success from 43% to 100%.

#### ✉️ [Guest Request Agent](https://github.com/vamsialladev/guest-request-agent) (stage 2)

**[▶ Watch the demo](https://vamsialla.com/projects/guest-request-agent.html#demo)** (AI-narrated) · **[Try the live app](https://guest-request-agent.streamlit.app)** (nothing is ever sent)

An agent reads a guest email, checks the booking and the hotel's policy, drafts a cited reply and proposes tasks;
staff approve, edit or reject every draft. Gated in CI at **100% escalation recall** and **100% prompt-injection
resistance**, with zero forbidden promises, at **$1.24 per 1,000 emails**.

#### 📏 [Eval Harness](https://github.com/vamsialladev/eval-harness) (stage 3)

**[▶ Watch the demo](https://vamsialla.com/projects/eval-harness.html#demo)** (AI-narrated) · **[Open the live dashboard](https://eval-harness.streamlit.app)** (read-only)

One evaluation system for both assistants. A "2 passages instead of 5" change stayed inside its confidence interval,
and the gate still failed it by name. An LLM judge agreed with my hand labels at kappa **0.29**, so I don't gate on it.

---

#### 🧰 Tools I work with
Python · Java · Claude API (tool use, structured outputs) · RAG (BM25 + embeddings) · MCP · Postgres / pgVector ·
Evaluation (Wilson intervals, kappa) · Streamlit · FastAPI · Playwright · AWS · Docker · GitHub Actions

#### 🧭 How I work
**Scope** the problem and what it costs → **build** with the data as it really is → **measure** with evals →
**deploy** under real limits → **hand over** docs the team can own.
