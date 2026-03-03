# The Three-Layer AI Risk Framework

> **Source:** BCS Session — "AI Compliance: Navigating the New Risk Landscape"
> **Speaker:** Bianca Chipanga
> **Host:** University of Hertfordshire × BCS – The Chartered Institute for IT
> **Date:** March 2026

---

## Why a Layered Model?

AI risk is not monolithic. The same organisation can simultaneously face three completely different risk profiles depending on *how* AI is being used and *by whom*. A flat, one-size-fits-all policy fails because the exposure, accountability, and remediation strategy differ entirely at each layer.

---

## Layer 1 — Employee-Facing AI Tools

**Definition:** AI applications accessed directly by staff for individual productivity, typically via personal or unmanaged accounts.

| Tool Type | Examples |
|---|---|
| General LLMs | ChatGPT, Microsoft Copilot, Google Gemini |
| Writing Assistants | Grammarly AI, Notion AI |
| Coding Tools | GitHub Copilot, Cursor |
| Summarisation Tools | Various browser extensions, Otter.ai |

### 🔴 Core Risk: Shadow AI
The barrier to entry is essentially zero. Staff can access powerful AI tools through a personal browser without any procurement, security vetting, or data processing agreement. This is **Shadow AI** — and it's the AI evolution of Shadow IT.

**Key consequence:** Sensitive corporate data (client information, internal strategy, source code) may be processed by external models without legal cover. The organisation has no visibility, no audit trail, and no recourse.

### ✅ Mitigation
- Audit current employee AI tool usage (surveys + network monitoring)
- Create an approved AI tools list with enterprise-grade data protection
- Choose vendors with explicit **opt-out clauses** for model training
- Establish a clear AI Acceptable Use Policy

---

## Layer 2 — AI Integrated within Vendor Products

**Definition:** "Hidden" AI functionality silently embedded in third-party software your organisation already uses and has already paid for.

### Where It Hides
- HR platforms (CV screening, performance analytics)
- CRM systems (lead scoring, sentiment analysis)
- Contract management tools (clause extraction, risk flags)
- Customer support platforms (chatbots, auto-routing)

### 🔴 Core Risk: Silent/Passive Adoption
This is the layer most organisations overlook. When a vendor pushes an update that activates an AI feature, **no new procurement cycle is triggered**. The AI enters your environment without a conscious decision being made. Your data may now be processed by third-party algorithms in ways your original data processing agreement never anticipated.

This directly risks:
- **Data residency violations** (data processed in a jurisdiction you didn't authorise)
- **UK GDPR non-compliance** (processing basis and purpose limitation)
- **Loss of organisational control** over how decisions affecting employees or customers are made

### ✅ Mitigation
- Audit all active software licences — flag any with AI/ML features (especially HR and CRM)
- Re-read data processing agreements with attention to AI-specific clauses
- Require vendors to disclose when AI features are added or modified
- Map all data flows to ensure residency and purpose compliance

---

## Layer 3 — Proprietary and Deployed AI Systems

**Definition:** AI systems built internally by the organisation, or AI used to make automated decisions that directly affect external stakeholders.

### High-Stakes Deployment Scenarios
1. **Credit** — Automated lending approvals and financial assessments
2. **Insurance** — Risk profiling, underwriting, and policy determination
3. **Hiring** — Candidate screening and selection
4. **Healthcare** — Clinical diagnostics or resource allocation

### 🔴 Core Risk: From Consumer to Operator
At this layer, the organisation is no longer just *using* AI — it is *responsible* for AI outcomes. Legal liability for algorithmic bias, discriminatory outputs, or opaque decisions now sits with the organisation. Regulatory scrutiny under the UK AI landscape (and EU AI Act for relevant organisations) is significant.

### ✅ Mitigation
- Implement a formal **AI Governance Programme**
- Mandate **bias testing** before any model deployment
- Enforce **human-in-the-loop** review for all customer-facing automated decisions
- Maintain transparency logs and audit trails for all model outputs

---

## Summary Table

| Layer | Risk Type | Who's Responsible | Urgency |
|---|---|---|---|
| 1 — Employee Tools | Shadow AI, data leakage | HR + IT Policy | 🔴 High |
| 2 — Vendor Products | Silent adoption, GDPR breach | Procurement + Legal | 🔴 High |
| 3 — Proprietary AI | Bias, liability, transparency | Executive + Legal + Engineering | 🔴 Critical |

---

## My Key Takeaway

> Layer 2 was the most eye-opening for me. Most compliance discussions focus on what employees *choose* to use (Layer 1) or what the organisation *builds* (Layer 3). But the silent creep of AI into tools already inside the perimeter — HR systems, CRMs — is happening *right now* without anyone pressing "approve." That's a governance gap hiding in plain sight.

---

*See also: [`case-studies/samsung-chatgpt-2023.md`](../case-studies/samsung-chatgpt-2023.md)*
