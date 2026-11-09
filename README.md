<h1 align="center">Ashish Ranjan</h1>

<p align="center">
  <b>I build AI agents that can act on real systems, and the guardrails that stop them doing damage.</b><br/>
  Forward Deployed Engineer intern at <a href="https://github.com/Infivector">Infivector</a> · IIT Patna '27 · India, open to remote
</p>

<p align="center">
  <a href="https://ashishranjan-ai.vercel.app"><img src="https://img.shields.io/badge/Portfolio-ashishranjan--ai.vercel.app-111?style=flat-square" alt="Portfolio"/></a>
  <a href="https://www.linkedin.com/in/ashish-ranjan6"><img src="https://img.shields.io/badge/LinkedIn-ashish--ranjan6-0A66C2?style=flat-square&logo=linkedin" alt="LinkedIn"/></a>
</p>

---

### How I build

An LLM is good at reading a messy situation and explaining it. It should not be the thing that moves money, deletes data or ships code with no checks. So everything I build has the same shape:

```
deterministic core  ──▶  LLM reasons and explains  ──▶  policy engine decides  ──▶  append-only audit log
  (finds the facts)       (never acts by itself)        (hard limits, idempotent)    (every step written once)
```

I build with coding agents every day. My part is the design, the diagnosis and checking the result against the real thing. On Limbo, the bugs that mattered showed up in runs against Razorpay's test mode, not in mocks.

### Now

- **Infivector, FDE intern (Jul 2026 to now).** Two-person team with the founder, so I own work end to end:
  - **AION**, an enterprise LLM gateway in Go: backend fixes, plus the benchmarking and acceptance-testing harness used in customer pilots. Public examples: [budget retry fix](https://github.com/ShubhamDX/aion/pull/19), [Bedrock response parsing](https://github.com/ShubhamDX/aion/pull/21), [budget tests](https://github.com/ShubhamDX/aion/pull/33).
  - **Conduit**, a desktop app that runs and manages coding agents: Windows support, agent adapters, connectors and status reporting. The repository is private.
- Final year of a BS in Computer Science and Data Analytics at **IIT Patna** (CPI 8.88).

### Selected work

| Project | What it is | Proof |
|---|---|---|
| [**Limbo**](https://github.com/ashish6123/limbo) | Agent that finds payments the gateway marked successful but the merchant never recorded, then recovers them: complete, replay the webhook, refund, or escalate. The LLM diagnoses. Only the policy engine can act. | [Live demo](https://limbo-ochre.vercel.app/demo): send a payment into limbo and watch it come back |
| [**ListingReel**](https://github.com/ashish6123/ListingReel) | Built alone: turns a real estate listing into a vertical video. LLM script, AI voiceover, FFmpeg captions. | [Live demo](https://listing-reel.vercel.app). Checkout runs in Razorpay test mode |
| [**Stadium Sentinel**](https://github.com/ashish6123/Stadium-Sentinel) | Multi-agent crowd safety system on Google ADK, Gemini and Vertex AI Search. A background monitor raises alerts before anyone asks. | **National finalist**, Google Cloud Agentic Premier League: top 80 of 3,000+ |
| [**TrustReview**](https://github.com/ashish6123/Trust-Review) | Fine-tuned DistilBERT that detects fake reviews, served as a FastAPI service. | 90.88% test accuracy, 60 tests, [live on HF Spaces](https://huggingface.co/spaces/rudra05/trust-review) |

### Upstream contributions

- **Kestra core fix, merged:** [stream `FilterItems` / `DeduplicateItems` records instead of loading the whole file into memory](https://github.com/kestra-io/kestra/pull/21997). Also merged: [unit tests for a UI widget](https://github.com/kestra-io/kestra/pull/21724) and a [Go benchmark regression gate blueprint](https://github.com/kestra-io/blueprints/pull/4831).

[![Kestra contributor](https://img.shields.io/badge/1st%20PR%20MERGED-KESTRA-1F232C?style=for-the-badge&logo=github&logoColor=200062&labelColor=CDC5FF)](https://kestra.io/community?from=github-badge)

### Toolbox

**Languages:** Python · Go · TypeScript · SQL
**AI:** Claude and Gemini APIs · Google ADK · Groq · Hugging Face · LLM gateways and routing · evals and benchmarking
**Backend:** FastAPI · PostgreSQL · Supabase · Next.js · Razorpay · Cloud Run · Render · Vercel

---

<p align="center"><i>Open to forward-deployed, AI and backend engineering roles. Remote contracts now (20 to 30 hrs/week), full-time from January 2027.</i></p>
