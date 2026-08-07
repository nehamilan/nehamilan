<H1>Hi there, I'm Neha 👋</H1> 

I'm a **product lead for national research data infrastructure** — a public, bilingual repository platform where research datasets are deposited, curated, published, and preserved. Some of that data is sensitive and governed by funder policy, so most of my job is deciding what a system is allowed to do on its own and where a human has to stand in the loop.

I build small AI products against the real problems that platform has. Each one ships with a product brief, not just a demo.

<H2> Projects</H2>

Every project here answers the same eight questions: what problem, what decision the model makes, what it may never output, how it's measured, what happens when it's unsure, where the human sits, what can go wrong, and what I traded away. The brief is the deliverable. The app or prototypes are proof the brief is real.

| Project | What it does | AI decision | Status |
| -------------- | --------------- | --------------- | ----------------- |			
| Intake Triage & Routing Assistant | Reads unstructured incoming requests and drafts a triage decision — category, priority, route, reason, confidence | Classification against a fixed controlled vocabulary; low-confidence and high-risk items escalate to a human queue instead of auto-routing | Completed |
| PulseReq | Replaces paper diagnostic requisitions with a tokenized, expiring link — the clinician orders by LOINC code, the patient books where and when, the lab receives a structured FHIR R4 `ServiceRequest` instead of re-keying a printed form | None — rules-based interoperability and workflow logic (embargo timers, link expiry, walk-in policy gating); no model-driven decision in current scope | In progress |

<H2>How I work</H2>

1. **I define the model's job narrowly before anyone builds.** Allowed outputs are a closed list. The constraint list — what it must never do — is written before the prompt is. Vague AI scope is where these projects die.
2. **I decide what happens when the model is wrong, because it will be.** Confidence threshold, escalation path, review queue. On the platform I run, a misrouted routine request costs a day; a mishandled sensitive-data request is a governance incident. Those are not the same error, so the system doesn't treat them the same. I optimize for the costly miss and accept false escalations.
3.  **Output is a draft until a human approves it.** Never presented as truth. Corrections feed back into the evaluation set.
4.  **I state the metric and the target before the build, not after the results.** Parse rate, precision, recall, a confusion matrix, and a stated reason for which one I'm optimizing.
5. **I write down what I gave up.** Every brief has a decisions-and-tradeoffs section, and a changelog showing the first accuracy number, the error pattern I found, the change I made, and the number after.

<H2>Background</H2>

- **Product Lead** on a national research data repository — own the product lifecycle end to end: strategy, requirements, specs, metrics, release. Sensitive-data deposit pathway, curation and preservation workflows, bilingual delivery, funder-policy compliance.
- **Previously Operations Lead** for the same service — SLAs with distributed infrastructure partners, change management, operational risk, and the transition from limited production to full national production.
- **Founded and chair a user community group** — 20+ researchers and librarians, quarterly. Their input has redirected real roadmap decisions, including a metrics-platform rebuild and a site redesign.
- **Founding member** of a national working group defining trustworthy-repository standards — persistent identifiers, preservation, metadata, cybersecurity, data-handling ethics, Indigenous data sovereignty, bilingualism. Designed and ran the group's member recruitment.
- **Co-chair** of Data Repository Expert Group (DREG). The DREG brings together representatives from key repository stakeholder communities to provide high-level coordination for platform-specific working groups and to foster a broad and cohesive approach to repository development in Canada.
- **Started in regulated systems** — delivery and project management on validated pharmaceutical systems, where every change carried an audit trail and "we'll fix it after launch" wasn't an available option. That's where the instinct for controlled vocabularies, approval gates, and provable decisions comes from.
- **Domains**: research data management, data governance, metadata standards, regulated and sensitive data.

<H2>What I'm looking for</H2>

AI product work where being wrong has consequences — regulated data, health, research, public infrastructure, banking. The interesting problem in those settings isn't model quality. It's deciding what the system is permitted to do unsupervised.
