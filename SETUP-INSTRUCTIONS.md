# Stage Canon — GitHub Setup Instructions

**For Luis**  
From: John / Cast Iron LA  
March 2026

---

## What This Is

Stage Canon is the public knowledge base for the Stage(TM) methodology. It lives on GitHub as a repository of markdown files — the methodology, glossary, examples, and tools.

Once it's on GitHub, any Claude session can be pointed to the raw file URL and will have full Stage context instantly. No more re-explaining the methodology at the start of every chat.

**This document tells you exactly what to do. Start to finish: about 10 minutes.**

---

## What's in the Zip

You have `stage-canon.zip`. Here's what's inside:

| File/Folder | What It Is |
|-------------|------------|
| **CONTEXT.md** | Session starter — paste this at the top of any new Claude chat to restore full project context instantly |
| **README.md** | Repo homepage — intro to Stage Canon, what it contains, how to use it |
| **SETUP-INSTRUCTIONS.md** | This file — setup instructions for you |
| **docs/methodology.md** | Complete Stage framework — Negative Anchor, resolution mechanics, all IP. THE most important file. |
| **docs/glossary.md** | Every Stage term defined — Negative Anchor, Resolution Architecture, Synthesis Gap, etc. |
| **docs/collapse-types.md** | The 5 collapse types mapped to the 5 Stage elements — diagnostic tool |
| **docs/qa-checklist.md** | 10 checks before publishing any staged page |
| **docs/faq.md** | Common questions about Stage — for us and for client education |
| **examples/ncg-case-study.md** | Complete NCG staging with results — the proof of concept |
| **examples/milk-sandwich.md** | Complete Milk Sandwich staging — reference implementation |
| **examples/integrare-draft.md** | Integrare staging in progress — includes diagnosis of their original copy |
| **tools/airtable-schema.md** | Vocabulary database setup and propagation options |
| **tools/stage-html-template.html** | Production HTML structure for staged pages — clean, semantic, ready to copy |
| **tools/brand-entropy-audit.md** | Brand Entropy Audit tool documentation |

---

## Setup — Step by Step

You need: a GitHub account (you have one), the `stage-canon.zip` file, about 10 minutes.

---

### Step 1 — Create the Repository

1. Go to **github.com** and sign in
2. Click the **+** icon in the top right → **New repository**
3. Repository name: **stage-canon**
4. Description: **Stage(TM) methodology — public knowledge base — Cast Iron LA**
5. Set to **Public** (this is required — AI needs to read it)
6. Check **"Add a README file"** — we'll replace it in a moment
7. Click **Create repository**

---

### Step 2 — Upload the Files

1. On your new repository page, click **Add file** → **Upload files**
2. **Unzip `stage-canon.zip` on your computer first**
3. Drag the **entire contents** of the `stage-canon` folder into the upload area — all files and folders at once
4. In the "Commit changes" box at the bottom, type: **Initial Stage Canon commit**
5. Click **Commit changes**

**Important:** Make sure you're uploading the **CONTENTS** of the `stage-canon` folder — not the folder itself. GitHub should show files like `README.md` and `CONTEXT.md` at the root level, with `docs/`, `examples/`, and `tools/` as folders.

---

### Step 3 — Verify the Structure

After uploading, your repository should look like this:

```
stage-canon/
  CONTEXT.md
  README.md
  SETUP-INSTRUCTIONS.md
  docs/
    methodology.md
    glossary.md
    collapse-types.md
    qa-checklist.md
    faq.md
  examples/
    ncg-case-study.md
    milk-sandwich.md
    integrare-draft.md
  tools/
    airtable-schema.md
    stage-html-template.html
    brand-entropy-audit.md
```

If it looks like that — you're done.

---

### Step 4 — Get the Raw URLs

The raw URL is what you paste into Claude. It gives Claude direct access to the file content.

**To get any raw URL:**
1. Click on the file in GitHub (e.g., `docs/methodology.md`)
2. Click the **Raw** button in the top right of the file view
3. Copy the URL from your browser — it will look like:

```
https://raw.githubusercontent.com/[your-username]/stage-canon/main/docs/methodology.md
```

---

### The Two URLs You'll Use Most

| URL | When to Use It |
|-----|----------------|
| **raw URL of CONTEXT.md** | Paste at the top of any new Claude session to restore full project context — client status, current work, file locations |
| **raw URL of docs/methodology.md** | Paste when you want Claude to have full Stage framework knowledge without the client context — useful for new client work or methodology questions |

---

## How to Use It in Claude

### Starting a New Session with Full Context

At the top of a new Claude chat, paste this exactly — replace `[URL]` with the raw CONTEXT.md URL:

```
Please read this file first, then confirm you have context:
[paste raw URL of CONTEXT.md here]
```

Claude will read the file and confirm it has full Stage context — current client work, methodology, file locations. You can then pick up exactly where you left off.

---

### Starting a Session for New Client Work

When starting a new client staging with no existing history:

```
Stage methodology reference: [paste raw URL of docs/methodology.md]

New client: [Client name]
Here is their current copy: [paste their copy]
Please diagnose and stage it.
```

---

### Asking a Methodology Question

If you're unsure about a Stage element or concept:

```
Using this as reference: [raw URL of docs/methodology.md]
Question: [your question]
```

---

### Getting a Specific Tool or Template

Need the HTML template or audit documentation?

```
Please read and provide:
[raw URL of tools/stage-html-template.html]
```

**Note:** Claude reads raw file URLs directly. You don't need to copy-paste the file contents — just the URL. This only works with **Public** repositories.

---

## Keeping It Updated

As Stage evolves — new clients, new examples, methodology refinements — the repo should stay current. Updating is simple.

### Adding a New Client Example

1. In GitHub, navigate to the `examples/` folder
2. Click **Add file** → **Create new file**
3. Name it: `[client-name].md` (lowercase, hyphenated)
4. Paste the staged content
5. Commit with message: **Add [Client] example**

---

### Updating an Existing File

1. Click on the file in GitHub
2. Click the **pencil (edit) icon** in the top right
3. Make your changes
4. Commit with a brief description of what changed

---

### Adding a New Methodology Doc

1. Navigate to the `docs/` folder
2. **Add file** → **Create new file**
3. Follow the same structure as existing docs — H1 title, Stage(TM) byline, sections
4. Add the new file to the table in `README.md` so it's discoverable

---

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
| Share repo with someone | `github.com/[your-username]/stage-canon` |

---

## After Setup

Once the repo is live:

1. **Send J. the repo URL** so it can be added to internal docs
2. **Test a raw URL** in a Claude session to confirm everything works
3. **Bookmark the repo** for quick access

That's it. The repo is now the single source of truth for Stage methodology.

---

**Stage Canon — Cast Iron LA**  
Questions during setup: bring them to a new Claude session with `CONTEXT.md` loaded.
