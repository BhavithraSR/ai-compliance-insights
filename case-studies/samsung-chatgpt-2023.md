# Case Study: Samsung ChatGPT IP Leak (2023)

> **Source:** BCS Session — "AI Compliance: Navigating the New Risk Landscape"
> **Relates to:** [Layer 1 — Employee-Facing AI Tools](../frameworks/ai-risk-three-layers.md)

---

## Incident Summary

**When:** Early 2023
**Who:** Engineers at Samsung Semiconductor
**What happened:** Engineers used ChatGPT to debug proprietary source code, directly entering confidential intellectual property into the third-party AI system.

---

## What Went Wrong

There was no internal gateway, no data loss prevention control, and no organisational policy in place at the time to prevent employees from pasting sensitive code into an external AI tool.

Three separate incidents were reported internally:
1. An engineer pasted confidential source code to ask ChatGPT to fix a bug
2. Another employee used it to optimise code, again sharing proprietary logic
3. A third used it to transcribe a confidential internal meeting

---

## The Impact

- **Hundreds of millions in R&D investment** potentially fed into a third-party model's training environment
- Once data enters an external LLM without opt-out protections, **data sovereignty is permanently lost**
- The now-famous quote from the incident sums it up:

> *"It left the building and it is not coming back."*

Samsung responded by banning the use of generative AI tools on company devices, and later began developing an internal AI system to avoid this class of risk entirely.

---

## Why This Matters for Cybersecurity Professionals

This isn't a hacking incident. No CVE. No malware. No threat actor.

The breach happened through **normal, well-intentioned employee behaviour** — engineers trying to do their jobs faster. That's what makes Shadow AI so dangerous and so hard to defend against with traditional security controls.

### The Security Stack That Didn't Help Here
- ✅ Firewalls — irrelevant (HTTPS to a legitimate domain)
- ✅ Antivirus — irrelevant (no malicious file)
- ✅ MFA — irrelevant (authenticated user)
- ❌ Data Loss Prevention — not configured for this vector
- ❌ AI Usage Policy — didn't exist yet
- ❌ Employee awareness — not trained for this risk

---

## Lessons for Organisations

| Lesson | Action |
|---|---|
| Assume employees will use AI tools | Audit usage *before* banning or policy-making |
| DLP rules need to cover AI endpoints | Update DLP to flag/block uploads to known LLM URLs |
| "Free" tools have hidden costs | Evaluate data training clauses in every AI tool's ToS |
| Speed-to-policy matters | Shadow AI moves faster than governance — act now |

---

## My Reflection

> This case study hit differently as someone who works in enterprise environments. The engineers weren't being reckless — they were being productive. That gap between *intent* and *impact* is exactly why governance frameworks need to be designed around human behaviour, not just technical controls. You can't patch culture with a firewall rule.

---

*Back to framework: [`frameworks/ai-risk-three-layers.md`](../frameworks/ai-risk-three-layers.md)*
