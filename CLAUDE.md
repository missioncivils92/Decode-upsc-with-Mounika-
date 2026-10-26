# CLAUDE.md

Instructions for Claude when working in this repository.

## What this repo is
The content workspace for **Decode UPSC with Mounika**, an English-language YouTube channel. Claude helps research, script and package videos. Read these first:
- `PLAYBOOK.md`: channel strategy, formats, templates, calendar. **Follow it.**
- `RESEARCH.md`: exam facts, audience research and sources.

## The channel in one paragraph
Mounika is a **mentor/educator** teaching **beginner aspirants (0–1 year into prep)** for **UPSC CSE (IAS/IPS/IFS)** and **State PSCs, with priority to APPSC and TGPSC** (Group 1/2), while keeping content useful to any state PSC. Videos are in **English**. Publishing cadence is **3 long videos per week: 2 explainers/exam guides + 1 weekly current-affairs roundup**, plus Shorts cut from them. The promise: _decode the exam into a clear, calm, step-by-step path._

## Audience: write for this person
A 20–24 year old graduate, often from a Tier-2/3 town, often first-generation, watching on a phone. Overwhelmed by too many sources. Wants to know what to do next, not everything at once. May be preparing for UPSC and APPSC/TGPSC together.

## Voice and style
- Speak as a mentor: warm, direct, confident; "you" and "we", never lecturing down.
- Plain English. Short sentences for the spoken script. Explain every acronym on first use (e.g., "CSAT, the second Prelims paper").
- Indian English and Indian number formats: lakh, crore; ₹.
- No hype or fear selling. No "crack UPSC in 3 months", no "guaranteed selection", no shaming.
- Be honest about the odds (about 0.1% of applicants are selected) and normalise having a backup plan.
- Politically neutral. Present government and opposition positions fairly; use official data. No party commentary.

## Accuracy rules (non-negotiable)
1. **Verify every exam date, vacancy count, rule, pattern and cut-off** against the official site (upsc.gov.in, psc.ap.gov.in, websitenew.tgpsc.gov.in) or PIB before it goes in a script. Coaching sites often disagree; never rely on a single one.
2. If something cannot be verified, say so in the script ("as per the last notification; check the new one") or leave it out. Never invent numbers, quotes, PYQs, or topper claims.
3. Cite sources for every current-affairs fact: PIB, PRS, The Hindu, Indian Express, government reports (Economic Survey, Budget, NITI Aayog, RBI). List them in the script's `sources` section.
4. When quoting a PYQ, give the exam and year (e.g., "UPSC Prelims 2023", "TGPSC Group 1 Mains 2024") and quote it exactly.
5. When `RESEARCH.md` facts go stale (new notification, result, calendar), update `RESEARCH.md` in the same change.

## How every explainer is built
Follow the "Decode Method" in `PLAYBOOK.md`:
**Hook → Why it matters for the exam → Concept (static) → Current link → PYQ → State PSC angle → Practice question → Next step.**

## Repository layout
```
CLAUDE.md          this file
PLAYBOOK.md        channel strategy and templates
RESEARCH.md        exam facts, audience research, sources
scripts/           one file per long video: YYYY-MM-DD-slug.md
shorts/            Shorts scripts: YYYY-MM-DD-slug-short-N.md
current-affairs/   weekly roundups: YYYY-Www-roundup.md (ISO week)
research/          topic research notes that feed scripts
```
Create folders as needed. Use lowercase, hyphenated slugs.

## Script file format
Every script in `scripts/` starts with this front matter:
```yaml
---
title: ""              # YouTube title, under 70 characters
format: explainer | ca-roundup | exam-guide
exams: [UPSC-CSE, APPSC, TGPSC]
syllabus: "GS II – Polity – Fundamental Rights"
target_length_min: 12
status: idea | research | draft | review | recorded | published
publish_date: YYYY-MM-DD
---
```
Then sections: `Hook`, `Script` (with on-screen text cues in `[brackets]`), `Shorts cuts` (2–4 timestamps or segments to reuse), `Thumbnail text` (3 options, max 4 words), `Description`, `Chapters`, `Tags`, `Sources`.

## When asked to create a video
1. Check `PLAYBOOK.md` for the format template and the content calendar.
2. Research; verify facts against official sources; record them in `research/` if substantial.
3. Write the script file in the format above.
4. Propose 2–4 Shorts cuts from it.
5. Flag anything unverified at the top of the file under `> VERIFY:`.

## Don'ts
- Don't write daily current-affairs videos unless asked; the default is the weekly roundup.
- Don't copy text from coaching material or newspapers; summarise and cite.
- Don't use Hindi or Telugu in titles or scripts unless asked (a term with English explanation is fine).
- Don't claim Mounika has a rank, selection or credential that hasn't been stated in this repo.
