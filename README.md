# Stage Canon

**The complete knowledge base for the Stage(TM) methodology**  
Cast Iron LA — March 2026

---

## What This Is

Stage Canon is the internal knowledge base for Stage — Cast Iron LA's proprietary AI search positioning methodology. This repository contains the complete framework, IP, examples, and tools.

**Purpose:** Any Claude session can be pointed to these raw file URLs and will have full Stage context instantly. No more re-explaining the methodology at the start of every chat.

**Audience:** Internal use — J., Luis, and any AI session working on Stage projects.

---

## What Stage Is

Stage is a methodology for positioning brands in AI search systems. Core insight: **AI systems function as probability-collapse engines, not retrieval systems.** Brands must optimize for selection, not visibility.

**Latest breakthrough (March 2026):**  
The **Negative Anchor effect** — AI systems weight criticism-with-resolution higher than praise alone. Resolution signals integrity. This insight led to a new product concept: **Resolution Architecture** — brands publicly documenting their own criticism, response, and change as a structured AI synthesis signal.

**Positioning:**
- Your website is where trust converts. Not where it starts. (SGO)
- Stage doesn't match the keyword. It matches the human who types it. (Stage)

---

## Repository Structure

### Core Documentation

| File | What It Contains |
|------|------------------|
| **[CONTEXT.md](CONTEXT.md)** | Session starter — paste at top of any Claude chat to restore full project context (clients, IP, file locations) |
| **[docs/methodology.md](docs/methodology.md)** | Complete Stage framework — Negative Anchor, resolution mechanics, S-T-A-G-E structure, all IP |
| **[docs/glossary.md](docs/glossary.md)** | Every Stage term defined — Negative Anchor, Resolution Architecture, Synthesis Gap, Echo Target, etc. |
| **[docs/collapse-types.md](docs/collapse-types.md)** | The 5 collapse types mapped to the 5 Stage elements — diagnostic tool |
| **[docs/qa-checklist.md](docs/qa-checklist.md)** | 10 checks before publishing any staged page |
| **[docs/faq.md](docs/faq.md)** | Common questions about Stage — for internal use and client education |

### Examples

| File | What It Contains |
|------|------------------|
| **[examples/ncg-case-study.md](examples/ncg-case-study.md)** | No Compromise Gaming — Stage30 proof of concept with results (+112% AI conversion lift, 1,295 sessions, 77 applications, $0 spend) |
| **[examples/milk-sandwich.md](examples/milk-sandwich.md)** | Complete Milk Sandwich staging — reference implementation |
| **[examples/integrare-draft.md](examples/integrare-draft.md)** | Integrare staging in progress — includes diagnosis of original copy |

### Tools

| File | What It Contains |
|------|------------------|
| **[tools/airtable-schema.md](tools/airtable-schema.md)** | Vocabulary database setup and propagation options |
| **[tools/stage-html-template.html](tools/stage-html-template.html)** | Production HTML structure for staged pages — semantic, clean, ready to copy |
| **[tools/brand-entropy-audit.md](tools/brand-entropy-audit.md)** | Brand Entropy Audit tool documentation — how it works, what it measures |

---

## How to Use This Repo

### Starting a new Claude session with full context

At the top of a new Claude chat, paste this:

```
Please read this file first, then confirm you have context:
https://raw.githubusercontent.com/[username]/stage-canon/main/CONTEXT.md
```

Claude will read the file and confirm it has full Stage context — current client work, methodology, file locations. You can pick up exactly where you left off.

### Starting a session for new client work

When staging a new client with no existing history:

```
Stage methodology reference:
https://raw.githubusercontent.com/[username]/stage-canon/main/docs/methodology.md

New client: [Client name]
Here is their current copy: [paste copy]
Please diagnose and stage it.
```

### Asking a methodology question

If you're unsure about a Stage element or concept:

```
Using this as reference:
https://raw.githubusercontent.com/[username]/stage-canon/main/docs/methodology.md

Question: [your question]
```

### Getting a specific tool or template

Need the HTML template or audit documentation?

```
Please read and provide:
https://raw.githubusercontent.com/[username]/stage-canon/main/tools/stage-html-template.html
```

**Note:** Claude reads raw file URLs directly. You don't need to copy-paste file contents — just the URL. This only works with Public repositories.

---

## Keeping It Updated

As Stage evolves — new clients, methodology refinements, IP development — this repo should stay current.

### Adding a new client example

1. Navigate to `examples/` folder in GitHub
2. Click **Add file → Create new file**
3. Name it: `[client-name].md` (lowercase, hyphenated)
4. Paste the staged content
5. Commit with message: `Add [Client] example`

### Updating an existing file

1. Click on the file in GitHub
2. Click the pencil (edit) icon
3. Make your changes
4. Commit with brief description

### Adding new IP or methodology updates

1. Update `docs/methodology.md` with new concepts
2. Add new terms to `docs/glossary.md`
3. Update `CONTEXT.md` if project status changes
4. Commit with clear description of what changed

**Every time you update a file, the raw URL stays the same.** Claude will always read the current version. No need to update your prompts when content changes.

---

## Quick Reference

| Task | How |
|------|-----|
| New Claude session with full context | Paste raw URL of `CONTEXT.md` + "Please read this first" |
| New client staging session | Paste raw URL of `methodology.md` + client copy + "please stage this" |
| Add new client example | GitHub → `examples/` → Add file → Create new file |
| Update existing content | GitHub → click file → pencil icon → edit → commit |
| Find a raw URL | GitHub → click file → **Raw** button → copy browser URL |
| Share repo | `github.com/[username]/stage-canon` |

---

## Current State (March 2026)

**Active clients:** No Compromise Gaming (proof of concept complete), Milk Sandwich  
**Major projects:** Adweek op-ed submission, Resolution Architecture product development, Hidden Hills RFP  
**Latest IP:** Negative Anchor effect, Resolution as primary AI signal, Section 31 five-claim set  
**Trademark:** Stage30 filed with USPTO (Section 1(b) Intent-to-Use)

---

**Stage Canon — Cast Iron LA**  
Questions or updates: bring them to a new Claude session with `CONTEXT.md` loaded.
