# Stage Canon — Introduction

**What it is, why it exists, how to use it**  
Cast Iron LA — March 2026

---

## The Problem It Solves

Every time you start a new Claude session, you lose context. You have to re-explain Stage methodology, re-list current clients, re-describe active projects, re-define terminology. Five minutes of setup before you can actually work.

**Stage Canon eliminates this.**

---

## What It Is

Stage Canon is a public GitHub repository containing the complete Stage methodology — framework, IP, examples, tools, current project state.

**Live at:** `github.com/jjbarbush/stage-canon`

Instead of re-explaining methodology at the start of every session, you paste one URL. Claude reads the file directly from GitHub and has instant, complete context.

---

## What's In It

### Core Documentation
- **CONTEXT.md** — Full project state: active clients, current work, IP development, file locations
- **methodology.md** — Complete Stage framework with Negative Anchor, resolution mechanics, all IP
- **glossary.md** — Every Stage term defined
- **collapse-types.md** — Diagnostic tool for identifying page failures
- **qa-checklist.md** — Pre-publish validation
- **faq.md** — Common questions about Stage

### Examples
- **NCG case study** — Proof of concept with results (+112% AI conversion lift)
- **Milk Sandwich** — Complete reference implementation
- **Integrare** — Work in progress with diagnosis

### Tools
- **Airtable schema** — Vocabulary database documentation
- **HTML template** — Production page structure
- **Brand Entropy Audit** — Synthesis resistance measurement

---

## How to Use It

### Starting a New Session with Full Context

At the top of any new Claude chat, paste this:

```
Please read this file first, then confirm you have context:
https://raw.githubusercontent.com/jjbarbush/stage-canon/main/CONTEXT.md
```

Claude reads the file and confirms it has:
- Current client status (NCG, Milk Sandwich, etc.)
- Active projects (Adweek submission, Resolution Architecture, Hidden Hills RFP)
- All Stage IP and terminology
- File locations in the repo

You can immediately pick up where you left off. No re-explaining.

---

### Starting Client Work (Without Full Context)

When you're staging a new client and don't need all the project baggage:

```
Stage methodology reference:
https://raw.githubusercontent.com/jjbarbush/stage-canon/main/docs/methodology.md

New client: [Client name]
Here is their current copy: [paste their copy]
Please diagnose and stage it.
```

Claude gets the framework without the project context.

---

### Asking a Methodology Question

If you're unsure about a Stage concept mid-session:

```
Using this as reference:
https://raw.githubusercontent.com/jjbarbush/stage-canon/main/docs/methodology.md

Question: What's the difference between Negative Anchor and Ambient Brand Weight?
```

---

### Getting a Specific Tool or Template

Need the HTML template or audit docs?

```
Please read and provide:
https://raw.githubusercontent.com/jjbarbush/stage-canon/main/tools/stage-html-template.html
```

---

## Why It Works

**Claude reads raw GitHub URLs directly.** You don't copy-paste file contents — you just paste the URL. Claude fetches the file and loads it into context.

**The URL never changes.** Every time you update a file on GitHub, that same URL serves the current version. Your prompts never need updating.

**It's public.** Anyone with the URL can access it. Internal use, but no authentication barriers.

---

## The Two URLs You'll Use Most

### 1. Full Context (Most Common)
```
https://raw.githubusercontent.com/jjbarbush/stage-canon/main/CONTEXT.md
```
Use this to restore full project state in any new session.

### 2. Methodology Only (New Client Work)
```
https://raw.githubusercontent.com/jjbarbush/stage-canon/main/docs/methodology.md
```
Use this when you need the framework but not the project context.

---

## Keeping It Current

As Stage evolves, update the repo. The workflow is simple:

### Adding a New Client Example
1. Go to `github.com/jjbarbush/stage-canon`
2. Navigate to `examples/` folder
3. Click **Add file** → **Create new file**
4. Name it `[client-name].md`
5. Paste the staged content
6. Commit with message: "Add [Client] example"

### Updating Existing Files
1. Click on the file in GitHub
2. Click the **pencil (edit)** icon
3. Make your changes
4. Commit with brief description

### Adding New IP
1. Update `docs/methodology.md` with new concepts
2. Add new terms to `docs/glossary.md`
3. Update `CONTEXT.md` if project status changed
4. Commit with clear description

**The raw URL stays the same.** Claude always reads the current version.

---

## What This Changes

### Before Stage Canon
- Start new Claude session
- Spend 5 minutes explaining Stage methodology
- Re-list current clients and projects
- Re-define terms as they come up
- Finally start actual work

### After Stage Canon
- Start new Claude session
- Paste CONTEXT.md URL
- Claude confirms context in 10 seconds
- Start actual work immediately

---

## Real Example

**You:** [Start new Claude chat]

```
Please read this file first, then confirm you have context:
https://raw.githubusercontent.com/jjbarbush/stage-canon/main/CONTEXT.md
```

**Claude:** "Context loaded. I have full Stage methodology, current client status (NCG proof of concept complete, Milk Sandwich active), active projects (Adweek submission, Resolution Architecture development, Hidden Hills RFP), and all Stage IP including Negative Anchor effect, Section 31 claims, and Larry/Gary model. Ready to work."

**You:** "NCG blog post. Topic: Why traditional lenders reject gamers. 800 words. Stage structure."

**Claude:** [Writes the post immediately with full Stage context, NCG voice, proper structure, no re-explaining needed]

---

## Quick Reference

| Task | URL to Use |
|------|-----------|
| Restore full project context | `CONTEXT.md` |
| Get Stage framework for new client | `methodology.md` |
| Look up term definition | `glossary.md` |
| Run diagnostic on weak page | `collapse-types.md` |
| Pre-publish validation | `qa-checklist.md` |
| Get HTML template | `tools/stage-html-template.html` |
| See proof of concept results | `examples/ncg-case-study.md` |

**All URLs start with:**
```
https://raw.githubusercontent.com/jjbarbush/stage-canon/main/
```

---

## The Bottom Line

Stage Canon is instant context for any Claude session. One URL, full methodology, zero setup time.

Instead of spending five minutes re-explaining Stage at the start of every chat, you paste one line and start working.

The repo is live. The methodology is documented. The examples are there. The tools are ready.

Just paste the URL and work.

---

**Stage Canon — Cast Iron LA**  
Live at: `github.com/jjbarbush/stage-canon`  
Questions: Load CONTEXT.md and ask
