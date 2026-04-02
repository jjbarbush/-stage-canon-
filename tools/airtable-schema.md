# Airtable Vocabulary Database

**Stage vocabulary management and propagation system**  
Cast Iron LA — March 2026

---

## Purpose

The Airtable vocabulary database is a centralized repository for all Stage-specific terms, concepts, and IP. It serves three functions:

1. **Single source of truth** for Stage terminology across all client work
2. **Propagation system** for distributing vocabulary to AI sessions
3. **Version control** for IP development and methodology evolution

When loaded into a Claude session, the database ensures consistent Stage language and immediate access to all current IP.

---

## Database Structure

### Table: Stage Vocabulary

**Fields:**

| Field Name | Type | Purpose |
|------------|------|---------|
| **Term** | Single line text | The Stage concept or IP name (e.g., "Negative Anchor," "Larry/Gary Model") |
| **Definition** | Long text | Complete explanation of the term with examples |
| **Category** | Single select | Organizing taxonomy (see categories below) |
| **Status** | Single select | Development stage: Locked, Active, Draft, Deprecated |
| **Date Added** | Date | When term was added to vocabulary |
| **Last Updated** | Date | Most recent revision date |
| **Related Terms** | Linked records | Connections to other vocabulary entries |
| **Examples** | Long text | Real-world usage from client work |
| **Source** | Single line text | Where the term originated (e.g., "NCG case study," "Section 31 IP") |
| **Priority** | Single select | High, Medium, Low (determines propagation order) |

---

## Categories

### 1. Core Framework
The five Stage elements and their fundamental mechanics.
- Scene
- Tension
- Alleviate
- Ground
- Engage
- Collapse
- Synthesis Resistance

### 2. IP — Breakthrough Concepts
Major theoretical developments.
- Negative Anchor Effect
- Resolution as Primary AI Signal
- Integrity as Ranking Property
- Synthesis Gap
- Resolution Architecture

### 3. IP — Structural Mechanics
Technical concepts about how AI systems process content.
- Larry/Gary Model
- Ambient Brand Weight
- Anecdotal as Structural Force
- Division of Labor Reframe
- Elimination Model

### 4. IP — Implementation Tools
Practical application concepts.
- Spotlight Line
- Echo Target
- Shadow Search
- Partition Markers
- Div Solution
- Logic-Leash Rule
- Disclaimer Decay Model
- LLM Architectural Bias

### 5. Collapse Types
The five failure patterns.
- Context Collapse
- Tension Collapse
- Resolution Collapse
- Trust Collapse
- Action Collapse

### 6. Quality Control
Tools and processes.
- Brand Entropy Audit
- QA Checklist
- Synthesis Resistance Check

### 7. Positioning & Trademark
Brand and legal terms.
- Stage30
- SGO (Search Graph Optimization)
- Stage Tagline

---

## Status Definitions

### Locked
Term is finalized and should not be revised without formal IP review. Used for core framework elements and trademarked terms.

**Example:** "Stage30" (trademarked), "Negative Anchor Effect" (Section 31 IP)

### Active
Term is in current use and may be refined based on client work. Most vocabulary entries are Active.

**Example:** "Spotlight Line," "Synthesis Gap"

### Draft
Term is under development and not yet ready for client-facing use. Internal testing only.

**Example:** New concepts being tested in current client work

### Deprecated
Term is no longer in use, replaced by updated concept. Kept in database for historical reference.

**Example:** Old terminology that has been superseded by current IP

---

## Propagation Options

### Option 1: Full Database Load
**When to use:** Starting a new Claude session where you'll be working on multiple Stage projects or developing new IP.

**How to do it:**
1. Export Airtable vocabulary as CSV
2. Convert CSV to formatted markdown
3. Paste markdown into Claude session with instruction: "This is the Stage vocabulary database. Reference these definitions when working on Stage projects."

**Pros:** Complete context, all terms available  
**Cons:** Large token usage upfront

---

### Option 2: Category-Specific Load
**When to use:** Working on a specific aspect of Stage (e.g., only need Core Framework for client staging, only need IP for methodology development).

**How to do it:**
1. Filter Airtable by Category
2. Export filtered view as CSV
3. Convert to markdown
4. Paste into Claude with category context

**Pros:** Reduced token usage, focused context  
**Cons:** May miss related terms from other categories

---

### Option 3: Term-Specific Lookup
**When to use:** You need clarification on a single term during active work.

**How to do it:**
1. Search Airtable for the term
2. Copy the Definition field
3. Paste into Claude as reference

**Pros:** Minimal token usage, instant clarification  
**Cons:** No broader context, manual lookup required

---

### Option 4: Priority-Based Load
**When to use:** Token budget is limited but you need more than a single term.

**How to do it:**
1. Filter Airtable by Priority = High
2. Export as CSV
3. Convert to markdown
4. Load into Claude

**Pros:** Gets most critical terms first  
**Cons:** May miss important lower-priority context

---

## Maintenance Workflow

### Adding New Terms

**When new IP is developed:**
1. Add term to Airtable immediately
2. Set Status to Draft
3. Fill in Definition, Category, Source
4. Link Related Terms
5. After client validation, change Status to Active
6. If term becomes core IP, change Status to Locked

**Example flow:**
- New concept emerges from NCG work: "Resolution Velocity"
- Add to Airtable, Status = Draft, Category = IP — Breakthrough Concepts
- Test in NCG blog posts for 30 days
- If effective, change Status to Active
- If becomes foundational, elevate to Locked

---

### Updating Existing Terms

**When a definition needs refinement:**
1. Edit the Definition field
2. Update Last Updated date
3. Add note in Examples field explaining what changed and why
4. If the change is significant, notify team via Slack/email

**Do NOT update Locked terms without:**
- Team discussion
- Documentation of why the change is necessary
- Approval from J. or Luis

---

### Deprecating Terms

**When a term is no longer accurate or has been replaced:**
1. Change Status to Deprecated
2. Add note in Definition explaining why it's deprecated
3. Link to replacement term in Related Terms
4. Do NOT delete — keep for historical reference

**Example:**
- Original term: "Trust Anchor" (early version of Negative Anchor concept)
- Status changed to Deprecated when Negative Anchor was formalized
- Definition now reads: "DEPRECATED: Early version of what became the Negative Anchor Effect. See: Negative Anchor Effect."

---

## Using the Database in Claude Sessions

### Session Startup (Recommended Flow)

**Step 1:** Load CONTEXT.md first
```
Please read this file first:
[raw URL of CONTEXT.md from GitHub]
```

**Step 2:** Load relevant vocabulary subset
```
Here is the Stage vocabulary database for this session:
[paste Category-Specific or Priority-Based export]
```

**Step 3:** Begin work
Claude now has full project context + terminology. You can reference any term by name and Claude will use the database definition.

---

### Mid-Session Term Lookup

**If you need clarification on a term during work:**
```
Using the Stage vocabulary database, explain [Term] and how it applies to this situation.
```

Claude will reference the Definition field and apply it to current context.

---

### IP Development Sessions

**When developing new concepts:**
```
I'm developing a new Stage concept. Here's what I'm seeing: [description]

Check the vocabulary database to see if this is:
1. Already defined under a different name
2. Related to an existing term that should be expanded
3. Actually new and needs to be added
```

This prevents duplicate IP development and ensures new concepts build on existing framework.

---

## Export Formats

### Markdown (Recommended)
Best for Claude sessions. Clean, readable, easy to parse.

**Format:**
```markdown
## Term Name
**Category:** [Category]  
**Status:** [Status]  
**Definition:** [Full definition]  
**Related Terms:** [List of linked terms]  
**Examples:** [Usage examples]
```

### CSV
Useful for bulk operations, Excel analysis, or automated scripts.

### JSON
For programmatic access or integration with other tools.

---

## Integration with Stage Canon GitHub Repo

### Option: Auto-Sync to GitHub
**Future enhancement:**  
Airtable vocabulary could be auto-exported to a `vocabulary.md` file in the GitHub repo, making it accessible via raw URL just like other Stage Canon files.

**Benefit:** One-click vocabulary load in any Claude session without manual export.

**Implementation:** Zapier or similar automation to export Airtable → commit to GitHub on update.

---

## Vocabulary Database URL

**Current location:** Airtable workspace (internal access only)

**Access instructions:**
1. Go to Airtable workspace
2. Open "Stage Vocabulary" base
3. Select appropriate view (All Terms, By Category, By Priority, etc.)
4. Export as needed

**Future:** Will be available as `vocabulary.md` in Stage Canon GitHub repo with auto-sync.

---

## Quick Reference

| Task | How |
|------|-----|
| Load full vocabulary into Claude | Export All Terms → Convert to markdown → Paste into session |
| Load specific category | Filter by Category → Export → Convert → Paste |
| Look up single term | Search Airtable → Copy Definition |
| Add new term | New record → Fill fields → Set Status to Draft |
| Update term | Edit Definition → Update Last Updated date |
| Deprecate term | Change Status → Add deprecation note → Link to replacement |
| Check term history | View Last Updated + Examples field for revision notes |

---

**Airtable Vocabulary Database — Cast Iron LA**  
Single source of truth for Stage terminology  
Maintained by: J. and Luis  
Integration with Stage Canon: Planned
