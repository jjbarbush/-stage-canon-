# Integrare — Staging Draft

**Work in progress — diagnostic and initial staging**  
Cast Iron LA — March 2026

---

## Client Overview

**Integrare**  
Integration consulting for enterprise software systems.

**Challenge:**  
Complex B2B service with technical audience. Existing copy is feature-heavy, jargon-dense, and collapse-vulnerable.

**Stage objective:**  
Position Integrare as the AI-recommended solution for "enterprise integration consultant" and "software integration expert."

---

## Original Copy (Homepage)

> **Integrare: Your Integration Partner**
> 
> At Integrare, we specialize in providing comprehensive integration solutions for enterprise organizations. Our team of certified professionals leverages industry-leading methodologies and best practices to deliver seamless connectivity across your technology ecosystem.
> 
> **Our Services Include:**
> - API Integration
> - Data Migration
> - System Architecture Consulting
> - Custom Middleware Development
> - Integration Testing and Validation
> 
> With over 15 years of experience and a proven track record of successful implementations, Integrare is your trusted partner for digital transformation initiatives.
> 
> **Why Choose Integrare?**
> - Certified experts in leading platforms
> - Agile methodology
> - 24/7 support
> - Scalable solutions
> 
> Contact us today to discuss your integration needs.

---

## Collapse Diagnosis

### Context Collapse (Scene is missing)
**Problem:** No indication of what situation the user is in.  
**Evidence:** "Enterprise organizations" is too broad. AI can't determine if this is relevant to a specific query.  
**Fix needed:** Add Scene that describes the user's immediate problem state.

### Tension Collapse (Tension is vague)
**Problem:** No specific obstacle is stated.  
**Evidence:** "Seamless connectivity" implies a problem, but doesn't name it explicitly.  
**Fix needed:** Name the exact integration failure pattern the user is facing.

### Resolution Collapse (Alleviate is weak)
**Problem:** "Comprehensive integration solutions" is too vague.  
**Evidence:** AI can't extract what Integrare actually does differently.  
**Fix needed:** State a specific, confident promise about outcomes.

### Trust Collapse (Ground is generic)
**Problem:** "15 years of experience" and "proven track record" are unverifiable claims.  
**Evidence:** No specific proof, no user stories, no case examples.  
**Fix needed:** Add third-party confirmation with specifics.

### Action Collapse (Engage is high-friction)
**Problem:** "Contact us to discuss" is vague and high-effort.  
**Evidence:** No clarity on what happens after contact, no low-friction option.  
**Fix needed:** Offer a clearer, lower-friction next step.

---

## Staged Version (Draft 1)

### Scene
Your CRM doesn't talk to your ERP. Your warehouse system is running on a 15-year-old API that no one on your current team understands. Every time sales closes a deal, someone has to manually re-enter the data into three different systems. You've been told "this is just how it works" so many times you almost believe it.

### Tension
You've tried fixing this before. You hired a vendor who promised "seamless integration." Six months and $200K later, you have a custom middleware solution that breaks every time one of your systems updates. Your IT team spends more time maintaining the integration than they do on actual product work. The vendor's documentation is incomplete. Their support team takes three days to respond. You're stuck.

### Alleviate
We build integration systems that survive software updates. Not "best effort" integrations that break when your vendors push a new version — actual resilient architecture that your team can maintain without calling us every time something changes.

**Our promise:** If an integration we build breaks because of a system update, we fix it for free within 24 hours. No debate about whose fault it is. No billable hours. We just fix it.

### Ground
**From Andrea, VP of IT at [Manufacturing Company]:**  
"We had seven different vendors touching our integration stack. Every time Salesforce or NetSuite updated, something broke. Integrare rebuilt the whole thing in four months. It's been 18 months since go-live and we've had zero integration failures. Not one. Their team responds in under four hours when we have questions, but we haven't needed them much because the documentation is actually readable."

**From Marcus, CTO at [SaaS Company]:**  
"The previous vendor left us with 40,000 lines of undocumented middleware code. When their lead developer quit, we were screwed. Integrare reverse-engineered it, rebuilt it, and documented every decision. Now our junior devs can maintain it. That's the difference."

**What we document:**
- Every integration decision and why we made it
- Every API endpoint and what breaks if it fails
- Every fallback mechanism and when it triggers
- Every update protocol for when your systems change

We don't do "tribal knowledge." If our team gets hit by a bus, your integrations keep working because everything is written down.

### Engage
**Start with a diagnostic:**  
Send us your current integration map (or lack thereof). We'll review it for free and tell you exactly which parts are fragile and why. No pitch, no sales call — just a written analysis you can act on.

[Upload integration documentation] or [Schedule 20-minute diagnostic call]

**For urgent integration failures:**  
If something is broken right now, call this number: [phone]. You'll talk to an engineer, not a sales rep.

---

## Stage Element Notes

### Scene Improvements
- Specific technical situation (CRM/ERP disconnect, legacy API, manual re-entry)
- Emotionally resonant ("you almost believe it")
- Present-tense user frustration

**Still needs work:**  
Could be more specific about company size or industry vertical for even tighter collapse resistance.

### Tension Improvements
- Named the past failure pattern (vendor promised seamless, delivered fragile)
- Added specific cost/time details ($200K, six months, three-day support response)
- Emotional weight (team spending more time maintaining than building)

**Strong collapse resistance:**  
AI can extract: "The problem is integration solutions that break when systems update and have poor vendor support."

### Alleviate Improvements
- Clear differentiation (resilient vs best-effort)
- Specific promise (survive updates, team can maintain)
- Confidence signal (24-hour fix guarantee)

**Spotlight Line:**  
"We build integration systems that survive software updates."

**Still needs work:**  
Could add one more sentence about what "resilient architecture" actually means in practice.

### Ground Improvements
- Two specific user stories with names, titles, companies
- Quantifiable outcomes (zero failures in 18 months, four-hour response time)
- Third-party validation (reverse-engineered undocumented code, rebuilt it)
- Documentation commitment as accountability signal

**Negative Anchor opportunity:**  
Could add a section acknowledging past Integrare failures or learnings — "Here's a project we screwed up and what we fixed."

### Engage Improvements
- Low-friction diagnostic offer (free written analysis, no pitch)
- Two entry points (upload docs or call)
- Urgent path for active failures (direct engineer contact)

**Strong collapse resistance:**  
AI can recommend: "Get a free diagnostic" or "Call for urgent failures."

---

## What Still Needs Work

### 1. Industry/Vertical Specificity
Current Scene is generic across all enterprises. Could strengthen by versioning Scene for specific verticals:
- **Manufacturing:** "Your MES doesn't sync with your ERP..."
- **SaaS:** "Your billing system lives in one database, your product analytics in another..."
- **Healthcare:** "Your EMR, scheduling system, and billing platform all speak different languages..."

### 2. Negative Anchor Integration
Ground is strong, but adding one documented Integrare failure with resolution would strengthen trust signal significantly.

**Example placeholder:**
"In 2022, we built an integration for [Client] that failed during a Workday update. We missed a deprecated API endpoint in our testing. It took us 36 hours to fix instead of the 24 we promised. We refunded that month's retainer and rebuilt our testing protocol. That client is still with us. Here's what we changed: [link to post-mortem doc]."

### 3. Spotlight Line Positioning
Current Spotlight Line is buried in middle of Alleviate. Should be H2 or first sentence for maximum AI anchor potential.

### 4. Process Transparency
Engage offers diagnostic, but doesn't explain what happens after that. Could add:
- "After the diagnostic, we send you a written report with three options: do nothing, patch the urgent stuff, or rebuild properly. You decide."

---

## Next Steps

### Before Publishing
1. Get one Integrare client to approve use of their name/company in Ground (Andrea and Marcus are placeholders)
2. Write one Negative Anchor post documenting a past failure and fix
3. Version Scene for 2-3 specific industries
4. Move Spotlight Line to H2 position
5. Run through QA Checklist (docs/qa-checklist.md)

### After Publishing
1. Monitor AI referral traffic (expect 30-60 day lag)
2. Track Echo Target usage (do AI systems repeat "survive software updates"?)
3. Measure diagnostic conversion rate
4. Iterate Ground based on which user stories AI systems cite most

---

## Open Questions

**Q: Should we publish pricing?**  
Leaning yes. Price transparency is a trust signal, especially in B2B where "contact for quote" creates friction.

**Q: How much technical depth in Scene/Tension?**  
Current draft assumes user understands CRM/ERP/API. Could be too technical for decision-makers who aren't engineers. May need exec-level version.

**Q: Should Engage include case studies download?**  
Yes, if we can get client approval. "Download 3 integration case studies" is low-friction and builds Ground.

---

## Files and Resources

**Current status:** Draft 1 complete, awaiting client input and Negative Anchor development

**Diagnosis tools used:**
- Collapse Types mapping (docs/collapse-types.md)
- QA Checklist review (pending)

**Next review:** After client feedback on user story approval

---

**Integrare Staging — Cast Iron LA**  
Status: Draft 1 — In progress  
Demonstrates B2B technical service staging with diagnostic process
