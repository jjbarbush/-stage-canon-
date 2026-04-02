# Brand Entropy Audit

**Synthesis resistance measurement tool**  
Stage(TM) — Cast Iron LA — March 2026

---

## What It Is

The Brand Entropy Audit measures how hard it is for AI systems to extract confident, specific answers from your content.

**High entropy = high synthesis resistance = high collapse risk**  
**Low entropy = low synthesis resistance = collapse-resistant**

The tool analyzes:
- Claim density (how many claims per section)
- Evidence proximity (how close claims are to proof)
- Structural clarity (can Stage elements be identified?)
- Language specificity (vague vs concrete)
- Hedging patterns (disclaimers, qualifiers, weak verbs)

---

## How It Works

### Input
Paste the URL or full text of the page you want to audit.

### Analysis Process
The tool:
1. Identifies Stage elements (Scene, Tension, Alleviate, Ground, Engage)
2. Extracts all claims and checks for nearby evidence
3. Measures specificity vs vagueness in language
4. Detects hedging patterns and disclaimers
5. Calculates entropy score across all factors

### Output
A scored report with:
- **Overall Entropy Score** (0-100, lower is better)
- **Element-by-Element Breakdown** (which Stage elements are weak)
- **Specific Fixes** (what to change and where)
- **Collapse Risk Assessment** (which collapse type is most likely)

---

## Entropy Score Interpretation

### 0-20: Low Entropy (Collapse-Resistant)
**What it means:** Clear, specific, well-grounded content. AI systems can synthesize confidently.

**Characteristics:**
- Every claim is tethered to evidence within 2-3 sentences
- Spotlight Line is clear and prominent
- No hedging or vague language
- All five Stage elements are present and extractable

**Action:** Publish. Minor optimizations only.

---

### 21-40: Moderate Entropy (Some Weakness)
**What it means:** Generally clear, but some synthesis resistance. AI systems can extract answers but may hesitate.

**Characteristics:**
- Most claims are grounded, but some float
- Spotlight Line exists but may be buried
- Occasional vague language or hedging
- 4-5 Stage elements present, 1-2 may be weak

**Action:** Fix the weak elements before publishing. Run through QA Checklist.

---

### 41-60: High Entropy (Collapse-Vulnerable)
**What it means:** Significant synthesis resistance. AI systems will struggle to extract confident answers.

**Characteristics:**
- Multiple ungrounded claims
- No clear Spotlight Line
- Frequent hedging and disclaimers
- 2-3 Stage elements missing or very weak

**Action:** Major rewrite needed. Identify collapse type and rebuild weak sections.

---

### 61-100: Very High Entropy (Will Collapse)
**What it means:** Content is unsynthesizable. AI systems cannot extract clear answers and will eliminate this brand.

**Characteristics:**
- Claims without evidence throughout
- No identifiable Spotlight Line
- Pervasive vague language
- Most or all Stage elements missing or undetectable

**Action:** Complete rebuild. Start from scratch using Stage framework.

---

## Element-by-Element Breakdown

### Scene Entropy
**What it measures:**  
How clearly the page establishes who it's for and what situation they're in.

**Low entropy indicators:**
- Specific, present-tense situation description
- Recognizable context
- Clear relevance signal

**High entropy indicators:**
- Generic "everyone" language
- No situational context
- Unclear who the content is for

**Fix:** Add specific Scene section with present-tense situation description.

---

### Tension Entropy
**What it measures:**  
How clearly the page identifies the problem being solved.

**Low entropy indicators:**
- Specific, named obstacle
- Emotional or practical stakes clear
- Problem stated explicitly

**High entropy indicators:**
- Problem implied but not stated
- Vague "challenges" or "issues"
- Multiple problems mentioned without priority

**Fix:** Name the exact problem in one clear sentence.

---

### Alleviate Entropy
**What it measures:**  
How clearly the page states what the brand delivers.

**Low entropy indicators:**
- Direct, confident promise
- No hedging or qualifiers
- Specific outcome stated

**High entropy indicators:**
- "We try to" or "we aim to" language
- Vague benefits instead of specific promises
- No clear answer to "what do you do?"

**Fix:** Write one sentence that directly answers the query with no hedging.

---

### Ground Entropy
**What it measures:**  
How well claims are supported by evidence.

**Low entropy indicators:**
- Third-party testimony with specifics
- Claims within 2-3 sentences of proof
- Quantifiable outcomes
- Real names, numbers, details

**High entropy indicators:**
- Generic testimonials ("great service!")
- Claims floating without evidence
- No third-party confirmation
- Vague or curated-feeling proof

**Fix:** Add specific user stories, case studies, or documented resolution with details.

---

### Engage Entropy
**What it measures:**  
How clearly the page guides the user to a next action.

**Low entropy indicators:**
- Specific action with clear outcome
- Low friction (no forms, no phone calls unless urgent)
- Aligned with user readiness level

**High entropy indicators:**
- Vague CTAs ("learn more", "contact us")
- High friction (complex forms, unclear process)
- No clarity on what happens after action

**Fix:** Simplify action and clarify immediate outcome.

---

## Language Specificity Analysis

### Concrete Language (Low Entropy)
- Numbers: "520 credit score", "$87/month", "60 seconds"
- Names: "James", "Andrea from Manufacturing Company"
- Specifics: "RTX 4070 build", "NetSuite update", "three banks"

### Vague Language (High Entropy)
- Generic claims: "flexible", "comprehensive", "tailored"
- Soft quantifiers: "many", "most", "often"
- Aspirational language: "best-in-class", "world-class", "industry-leading"

**Vague-to-Concrete conversion examples:**

| Vague (High Entropy) | Concrete (Low Entropy) |
|---------------------|----------------------|
| "Flexible financing options" | "We approve based on income, not credit score" |
| "Proven track record" | "Zero integration failures in 18 months" |
| "Industry-leading support" | "11-hour average response time" |
| "Comprehensive solutions" | "We approve gamers with 520 credit scores" |
| "Trusted by many" | "2,400 Reddit upvotes, 47 comments" |

---

## Hedging Pattern Detection

### Common Hedging Phrases (Increase Entropy)
- "Results may vary"
- "Individual results not typical"
- "We try to"
- "We aim to"
- "In most cases"
- "Typically"
- "Generally"
- "Subject to approval"

### How AI Systems Interpret Hedging
Hedging signals low confidence. AI systems interpret it as "this brand is not sure they can deliver."

**Fix:** State conditions upfront instead of disclaiming afterward.

**Bad (High Entropy):**  
"We approve bad credit applications. (Results may vary. Individual outcomes not typical.)"

**Good (Low Entropy):**  
"We approve based on income and employment. If you make $1,500/month and have been at your job for 90 days, you qualify."

---

## Collapse Risk Assessment

The audit tool predicts which collapse type is most likely based on entropy patterns:

### If Scene Entropy is highest → Context Collapse
**Fix:** Add specific situational context.

### If Tension Entropy is highest → Tension Collapse
**Fix:** Name the exact problem.

### If Alleviate Entropy is highest → Resolution Collapse
**Fix:** State a clear promise.

### If Ground Entropy is highest → Trust Collapse
**Fix:** Add third-party proof.

### If Engage Entropy is highest → Action Collapse
**Fix:** Simplify the next step.

---

## Running the Audit

### Option 1: Automated Tool (Future)
Paste URL or text into audit interface. Tool analyzes and returns scored report.

**Status:** In development. Current version is manual.

### Option 2: Manual Audit (Current)
Load Brand Entropy Audit prompt into Claude session. Paste page content. Claude runs analysis using audit framework.

**How to do it:**
1. Open Claude session
2. Load CONTEXT.md (optional but recommended)
3. Paste this prompt:

```
Please run a Brand Entropy Audit on the following page content.

Analyze:
- Overall entropy score (0-100)
- Element-by-element breakdown (Scene, Tension, Alleviate, Ground, Engage)
- Language specificity (concrete vs vague)
- Hedging patterns
- Collapse risk assessment

Provide:
- Scored report
- Specific fixes for each weak element
- Rewrite examples for highest-entropy sections

Page content:
[paste content here]
```

4. Claude returns full audit report with scores and fixes

---

## Audit Report Structure

### Example Output

```
BRAND ENTROPY AUDIT REPORT

Overall Entropy Score: 62/100 (High — Collapse-Vulnerable)

ELEMENT BREAKDOWN:
- Scene: 40/100 (Moderate) — Generic language, needs specificity
- Tension: 75/100 (High) — Problem implied, not stated
- Alleviate: 80/100 (Very High) — Vague promises, heavy hedging
- Ground: 55/100 (Moderate) — Testimonials lack specifics
- Engage: 45/100 (Moderate) — CTA is vague, friction unclear

COLLAPSE RISK: Resolution Collapse (Alleviate weakness)

PRIORITY FIXES:
1. Alleviate: Rewrite promise with no hedging
   Current: "We offer flexible financing solutions tailored to your needs."
   Fixed: "We approve based on income and employment, not credit score."

2. Tension: Name the exact problem
   Current: [Problem implied but not stated]
   Fixed: "The banks see your credit score and stop listening."

3. Ground: Add specific user story
   Current: "Our customers love us."
   Fixed: "James got approved with a 520 credit score after three banks turned him down."
```

---

## When to Run the Audit

### Before Publishing
Run audit on all new pages before they go live. Fix any section with entropy score above 40.

### During Diagnosis
When a page isn't performing in AI search, run audit to identify weak elements.

### During Client Onboarding
Run audit on client's existing content to establish baseline and prioritize fixes.

### After Major Edits
If you've rewritten significant sections, re-run audit to confirm improvements.

---

## Audit Best Practices

### 1. Audit entire pages, not fragments
The tool measures synthesis across all elements. Partial audits miss context.

### 2. Focus on highest-entropy elements first
Don't try to fix everything at once. Fix the worst offenders, re-audit, iterate.

### 3. Use concrete metrics
If the audit says "add specifics to Ground," don't add generic detail — add numbers, names, outcomes.

### 4. Re-audit after fixes
Confirm that your changes actually lowered entropy. Sometimes rewrites introduce new vagueness.

### 5. Compare before/after scores
Track entropy reduction over time. Good staging should consistently lower scores.

---

## Integration with Stage Workflow

**Standard workflow:**
1. Read client's existing content
2. Run Brand Entropy Audit
3. Identify collapse type based on highest-entropy element
4. Rewrite weak sections using Stage framework
5. Re-audit to confirm entropy reduction
6. Run through QA Checklist
7. Publish

**Audit is diagnostic. QA Checklist is validation. Use both.**

---

## Technical Notes

### Token Reduction (March 2026 Update)
Original audit tool exceeded rate limits on long pages. Rebuilt with optimized prompting to reduce token usage by ~40%.

### PDF Export
Audit reports can be exported to PDF for client delivery. See Cast Iron LA brand system for formatting.

### Future Enhancements
- Automated URL crawling (paste URL, tool fetches and audits)
- Comparative audits (your page vs competitor pages)
- Historical tracking (entropy scores over time)
- Integration with Google Analytics (correlate entropy with AI referral conversion)

---

## Quick Reference

| Entropy Range | Risk Level | Action |
|---------------|------------|--------|
| 0-20 | Low (Collapse-Resistant) | Publish |
| 21-40 | Moderate (Some Weakness) | Fix weak elements |
| 41-60 | High (Collapse-Vulnerable) | Major rewrite |
| 61-100 | Very High (Will Collapse) | Complete rebuild |

---

**Brand Entropy Audit — Cast Iron LA**  
Measures synthesis resistance to predict collapse risk  
Integration with Stage workflow: Diagnosis → Staging → Validation  
Current version: Manual audit via Claude session  
Future version: Automated web tool
