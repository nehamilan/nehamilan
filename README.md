<H1>Hi there, I'm Neha 👋</H1> 

I **build systems that make consequential decisions on unstructured input** — classify against a controlled vocabulary, apply the rules deterministically, and escalate to a human when confidence is low or the stakes are high. I do it today on national research data infrastructure, where some data is sensitive and governed by funder policy. The pattern is the same in claims, in AML alerts, and in vendor risk review.

I build AI/traditional products against problems in regulated environments. Each one ships with a product brief, not just a demo.

<H2> Projects</H2>

Every project here answers the same eight questions: what problem, what decision the model makes, what it may never output, how it's measured, what happens when it's unsure, where the human sits, what can go wrong, and what I traded away. The brief is the deliverable. The app or prototypes are proof the brief is real.

**When I use a model and when I don't:** an LLM when the input is unstructured, the output space is closed, and a wrong answer is recoverable in human review. Deterministic rules when the decision is enumerable, legally binding, or has to be reproducible in an audit.

| Project | What it does | Why AI/Why not | Status | Transfers to |
| -------------- | --------------- | --------------- | ----------------- | ----------------- |				
| Intake Triage & Routing Assistant | Reads unstructured incoming requests and drafts a triage decision — category, priority, route, reason, confidence | Input is unstructured, output space is closed, errors are recoverable in review — LLM | Completed | AML alert triage, phishing report triage |
| PulseReq | Replaces paper diagnostic requisitions with a tokenized, expiring link — the clinician orders by LOINC code, the patient books where and when, the lab receives a structured FHIR R4 `ServiceRequest` instead of re-keying a printed form | Every decision is enumerable and must be reproducible in audit — deterministic rules, no model | In progress | Payment authorization links, time-bound access grants |

**Intake Triage & Routing Assistant**

**Pattern:** unstructured intake → classification against a closed vocabulary → confidence-gated routing → human review queue for the costly misses.
**Same shape elsewhere:** AML alert triage in banking, where a false negative is a regulatory finding and a false positive is an analyst hour. Phishing-report triage in security operations, where the reported-email queue has to be sorted before anyone can act on it.

**PulseReq**

**Pattern:** replace a paper artifact with a tokenized, expiring link → structured payload to the receiving system → policy enforced as workflow rules, not judgment.
**Same shape elsewhere:** payment-authorization links in fintech, where the token's expiry is the control. Time-bound access grants in security, where entitlement, expiry, and revocation must be provable after the fact.

<H2>How I work</H2>

1. **I define the model's job narrowly before anyone builds.** Allowed outputs are a closed list. The constraint list — what it must never do — is written before the prompt is. Vague AI scope is where these projects die.
2. **I decide what happens when the model is wrong, because it will be.** Confidence threshold, escalation path, review queue. On the platform I run, a misrouted routine request costs a day; a mishandled sensitive-data request is a governance incident. Those are not the same error, so the system doesn't treat them the same. I optimize for the costly miss and accept false escalations.
3.  **Output is a draft until a human approves it.** Never presented as truth. Corrections feed back into the evaluation set.
4.  **I state the metric and the target before the build, not after the results.** Parse rate, precision, recall, a confusion matrix, and a stated reason for which one I'm optimizing.
5. **I write down what I gave up.** Every brief has a decisions-and-tradeoffs section, and a changelog showing the first accuracy number, the error pattern I found, the change I made, and the number after.

<H2>Background</H2>

- **Product Lead, national research data repository.** Own the lifecycle end to end — strategy, requirements, specs, metrics, release. Sensitive-data deposit pathway, curation and preservation workflows, funder-policy compliance, bilingual delivery. Decisions here are governed: what the system may do unsupervised is a policy question before it is a technical one.
- **Started in validated pharmaceutical systems.** Delivery and project management where every change carried an audit trail and "we'll fix it after launch" wasn't available. Controlled vocabularies, approval gates, and provable decisions are instincts from there, not vocabulary I picked up for AI work.
- **Founding member, national working group on trustworthy-repository standards.** Persistent identifiers, preservation, metadata, cybersecurity, data-handling ethics, Indigenous data sovereignty, bilingualism. Designed and ran member recruitment. Writing the standard is a different skill from meeting one.
- **Chair, 20+ member researcher and librarian community; co-chair, Data Repository Expert Group.** Direct user input has redirected real roadmap decisions, including a metrics-platform rebuild and a site redesign. Both roles are coordination across stakeholder groups with competing requirements.
- **Domains**: research data management, data governance, metadata standards, regulated and sensitive data.

AI product work where being wrong has consequences — regulated data, health, research, public infrastructure, banking. In these settings the interesting problem isn't model quality. It's deciding what the system is permitted to do unsupervised.
