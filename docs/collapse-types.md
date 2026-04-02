# Collapse Types

**Diagnostic tool for identifying why pages fail in AI search**  
Stage(TM) — Cast Iron LA — March 2026

---

## Overview

Every weak page collapses for one of five reasons. Each collapse type maps directly to a Stage element.

This document is a diagnostic tool. Read the brand's existing page. Identify which collapse type is causing failure. Fix the corresponding Stage element.

---

## The Five Collapse Types

### 1. Context Collapse
**What it is:** The AI can't determine if the content is relevant to the user's query.

**Why it happens:**
- Generic language that could apply to anyone
- No clear indication of who the content is for
- Missing situational anchors that connect to the search moment

**Example of Context Collapse:**
"We offer financing solutions for your needs."  
(For what? In what situation? The AI has no way to know if this is relevant.)

**Stage element that fixes it:** **Scene**

**How to fix:**
Write a specific, present-tense Scene that describes the exact situation the user is in when they search.

**After fix:**
"You want to finance a gaming PC. You're 19, you work part-time, your credit score is 580, and every lender you've tried has said no."

**Test:** Can the AI confidently say "this content is for someone in [specific situation]"? If no, it's Context Collapse.

---

### 2. Tension Collapse
**What it is:** The AI can't identify what problem the brand solves.

**Why it happens:**
- The problem is implied but never stated
- The language is too vague to pin down a specific obstacle
- Multiple problems are mentioned without clear prioritization

**Example of Tension Collapse:**
"Financing can be complicated and confusing."  
(What exactly is the problem? Why is it complicated? The AI can't extract a specific obstacle.)

**Stage element that fixes it:** **Tension**

**How to fix:**
Name the exact, unresolved problem the user is trying to solve. Must be specific and stated as an obstacle.

**After fix:**
"The banks don't care that you have a job and pay your bills. They see your score and stop listening."

**Test:** Can the AI complete this sentence: "This brand solves the problem of [specific obstacle]"? If no, it's Tension Collapse.

---

### 3. Resolution Collapse
**What it is:** The AI can't extract a clear answer or promise.

**Why it happens:**
- The brand hedges with "we try to" or "we aim to"
- The solution is described in vague, aspirational language
- No confident, actionable statement of what the brand delivers

**Example of Resolution Collapse:**
"We offer flexible financing options to help you achieve your goals."  
(What does "flexible" mean? What exactly do you do? The AI has no specific answer to extract.)

**Stage element that fixes it:** **Alleviate**

**How to fix:**
Write a direct, confident statement of what the brand promises. No hedging, no vague benefits.

**After fix:**
"We approve based on income and employment, not credit score. If you make $1,500/month and have been at your job for 90 days, you qualify."

**Test:** Can the AI confidently say "this brand promises [specific outcome]"? If no, it's Resolution Collapse.

---

### 4. Trust Collapse
**What it is:** The AI can't verify the brand can deliver on its promise.

**Why it happens:**
- No evidence, proof, or third-party confirmation
- Claims float without grounding
- Testimonials feel curated or generic
- No documentation of accountability or past resolution

**Example of Trust Collapse:**
"Our customers love us and we have a high satisfaction rate."  
(Says who? Where's the proof? The AI has nothing to verify this claim.)

**Stage element that fixes it:** **Ground**

**How to fix:**
Add third-party confirmation: user stories with specifics, reviews, case studies, or publicly documented resolution of past criticism.

**After fix:**
"James got approved with a 520 credit score. He'd been turned down by three banks. Now he's gaming on a custom rig he's paying off at $87/month."

**Test:** Can the AI point to specific evidence that proves the brand can deliver? If no, it's Trust Collapse.

---

### 5. Action Collapse
**What it is:** The AI can't recommend a next step to the user.

**Why it happens:**
- The call-to-action is vague ("learn more," "contact us")
- Too much friction (forms, phone calls, unclear process)
- No clarity on what happens after the user acts

**Example of Action Collapse:**
"Contact us today to learn more about our financing options."  
(What does "contact" involve? What happens next? The AI can't guide the user forward.)

**Stage element that fixes it:** **Engage**

**How to fix:**
Write a frictionless, immediate action aligned with the user's readiness level. Be specific about what happens.

**After fix:**
"Check if you're pre-approved in 60 seconds. No credit pull. No obligation."

**Test:** Can the AI confidently tell the user "do [specific action] next"? If no, it's Action Collapse.

---

## Diagnostic Process

### Step 1: Read the page
Read it as an AI would — looking for clear, extractable answers.

### Step 2: Ask the synthesis question
"If an AI had to explain what this brand does and why someone should choose it, could it?"

### Step 3: Identify the collapse type
If the answer is no, determine which element is weak:
- Can't tell who this is for? → Context Collapse (Scene is weak)
- Can't identify the problem? → Tension Collapse (Tension is weak)
- Can't extract a clear promise? → Resolution Collapse (Alleviate is weak)
- Can't verify the brand can deliver? → Trust Collapse (Ground is weak)
- Can't recommend a next step? → Action Collapse (Engage is weak)

### Step 4: Fix the corresponding Stage element
See methodology.md for detailed rules on how to write each element.

### Step 5: Re-test
Read the revised page and ask the synthesis question again. If the AI could now confidently synthesize, the collapse is fixed.

---

## Multiple Collapse Types

Some pages collapse for multiple reasons. Fix them in order:
1. **Context Collapse** (Scene) — without this, nothing else matters
2. **Tension Collapse** (Tension) — the AI needs to know what problem to solve
3. **Resolution Collapse** (Alleviate) — the AI needs a clear answer
4. **Trust Collapse** (Ground) — the AI needs proof
5. **Action Collapse** (Engage) — the AI needs a next step to recommend

---

## Common Patterns

### Brand pages that collapse on Ground
Most common failure. The brand makes bold claims but provides no evidence. AI can't verify, so it seeks external sources — often finding contradictory information.

**Fix:** Add user stories, reviews, case studies, or documented resolution of past criticism.

### Landing pages that collapse on Alleviate
The brand describes benefits but never states a specific promise. AI can't extract a clear answer.

**Fix:** Write one sentence that directly answers "what do you do?" with no hedging.

### Product pages that collapse on Scene
The page assumes the reader already knows why they're there. AI can't connect the content to the user's query.

**Fix:** Add context at the top that describes the specific situation this product is for.

### Service pages that collapse on Tension
The page lists features but never names the problem. AI can't identify what obstacle this solves.

**Fix:** State the exact problem before describing the solution.

### Contact pages that collapse on Engage
"Get in touch" is too vague. AI doesn't know what action to recommend or what outcome to promise.

**Fix:** Be specific about what happens after contact and what the user can expect.

---

## Collapse Type Summary Table

| Collapse Type | AI Can't Extract | Stage Element | Quick Fix |
|---------------|------------------|---------------|-----------|
| **Context Collapse** | Relevance to user's situation | **Scene** | Add specific, present-tense context |
| **Tension Collapse** | The problem being solved | **Tension** | Name the exact obstacle |
| **Resolution Collapse** | A clear promise or answer | **Alleviate** | State what you deliver, no hedging |
| **Trust Collapse** | Proof the brand can deliver | **Ground** | Add third-party evidence |
| **Action Collapse** | What the user should do next | **Engage** | Simplify the next step |

---

**Collapse Types — Cast Iron LA**  
For full methodology: see `docs/methodology.md`  
For practical examples: see `examples/` folder
