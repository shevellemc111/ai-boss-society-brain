---
name: business-brain-builder
description: Required. Builds business-brain.md — the operating brain your AI employees run on. Use at the start of Business Brain pre-work, whenever business-brain.md doesn't exist yet, or needs a refresh. ~20-25 minutes. Trigger on "business brain," "start my business brain," "let's do my business brain," "business brain pre-work," or any request to build, fill out, or create a business brain file.
---

# Business Brain Builder

This skill builds `business-brain.md` — the single file your three AI employees (Intake Coordinator, Email Manager, Operations Assistant) read before doing anything. It is the business equivalent of a new hire's training manual: what you do, who you do it for, how you sound, how work actually flows, and where the hard lines are.

This is a **required** module. Budget 20-25 minutes. The goal is a usable first draft — you can always refine it later, so don't let a tricky question stall you out.

## Before you start

Check whether `business-brain.md` already exists in this workspace (usually under `about-me/business-brain.md` or wherever this training's files are being kept). Check also whether the person has a completed **Business Brain Prep Sheet** (the fillable Word doc version) — either uploaded as a file, pasted into the chat, or mentioned as "I filled this out already." Also ask whether they'd rather talk through their answers than type them — see **Voice memo option** below.

Then pick a path:

- **No existing file, no Prep Sheet, no voice memo → Path A (Interview).**
- **A completed (or partially completed) Prep Sheet, or a voice memo transcript, exists → Path B (Gap-Check).**
- **`business-brain.md` already exists → tell them what you found and ask if they want to redo it fully (Path A), gap-check it against the current questions (Path B logic, using the existing file as the "prep sheet"), or leave it alone.**

Never assume — ask in one line if it's not obvious which path applies.

### Voice memo option

Some people find it easier to talk through this than type it. Offer it as an alternative up front: "If you'd rather talk through this than type, record yourself out loud answering the Business Basics and the 9 questions — your phone's voice memo app is the easiest way, or your computer's dictation/recording tool if that's easier for you. Most transcribe automatically; if not, dictate straight into a Notes app. Upload or paste the resulting transcript here instead of doing the typed interview."

Treat an uploaded transcript as a Path B input, same as a Prep Sheet — see the transcript-specific notes under Path B below. A rambling spoken transcript won't be organized by question number the way a Prep Sheet is, so it needs a mapping step the Prep Sheet doesn't.

**Bonus:** if this person also needs the Writing Rules module, their Business Brain voice memo transcript can double as that module's required "transcript / spoken-to-written" sample — mention this so they don't have to record a second one. Flag it to the writing-rules-builder skill (or just note it in business-brain.md) rather than making them repeat themselves.

---

## Path A — Interview (default, no prep sheet)

Walk through Business Basics, then the 9 core questions, **one at a time**. Do not front-load all 9 questions in one message — this is a conversation, not a form dump.

After EVERY answer (including each Business Basics field), write it to `business-brain.md` immediately using the template below before asking the next question. Don't batch writes to the end — if the session gets interrupted, whatever's answered so far should already be saved.

### Step 0 — Business Basics

Ask for these together, since they're quick facts, not reflection:

1. Your name
2. Your role/title (owner, coach, founder, etc.)
3. Business name
4. Industry / niche (be specific — "travel advisor," "1:1 life coach," "solo accountant," "residential realtor," not "service business")
5. Business size (solo, or team — and if team, roughly how many)

Write these into the **Business Basics** section of the template immediately.

### Step 1 — The 9 core questions

Ask each of these as its own message. Wait for the answer, write it to file, then move to the next. Light follow-up is fine if an answer is thin (e.g., "anything else that's off the table?") but don't turn this into a 20-question interrogation — keep momentum.

**Q1 — Services & scope**
"What services do you offer, and what's explicitly not something you do? For each service line, list the specific offerings within it, anything you've stopped offering, and anything you deliberately keep off the table."

**Q2 — Ideal client & result**
"Describe your ideal client in concrete terms, and the result you actually deliver for them. What problem or fear brings them to you? What's different for them once you're done? And who is NOT a fit — both situational mismatches (wrong budget, wrong stage, wrong industry) and behavioral ones (high-maintenance, distrustful, excessive contact)?"

**Q3 — Communication style**
"Describe how you actually sound when you write to clients — your tone, your go-to phrases or sign-offs — and give me one or two short example lines you'd genuinely say (a phrase or two, not a full message). What would sound obviously wrong coming from you?"

Then say: "Now let's sanity-check your voice against a starter list of things that make writing sound AI-generated. Read through it and tell me what to cut, what to keep, and anything you'd add." Paste the **Starter Anti-AI Kill List** below as a code block. Let them edit it live in conversation — don't ask them to write a list from scratch. Write their edited version into the file.

> **Note:** This captures a quick tone description, not a full writing sample — the required Writing Rules module is where the real samples live (three of them, across client-facing, social, and transcript/spoken registers). Don't ask for a full sample here; that's Writing Rules' job. If they've already built writing-rules.md, pull the tone description from there instead of re-asking — say "since you already built writing-rules.md, I'll pull your tone from there" and move straight to the Kill List check.

**Q4 — Client journey**
"Walk me through the full journey, from first contact through the engagement wrapping up: how clients find you, the path to a signed agreement (and anything else that disqualifies someone along the way), whether the process branches depending on the type of service, what happens during the engagement itself, how it actually ends, and what happens if a client needs to end early."

**Q5 — Recurring communications**
"What are the messages or check-ins you send over and over? Which of those need your personal review before they go out?"

**Q6 — Team & tools**
"Who's on your team and what do they own? Solo is a completely valid answer. Who handles what — you, a VA, contractors? What channels do you communicate through, and what software runs your business?"

**Q7 — AI boundaries & escalation**
"What should AI never do on its own, no exceptions? Who does it escalate to when something's outside its lane? Any capacity limits worth flagging — how many clients you can take on, busy seasons, anything like that?"

**Q8 — Pricing structure**
"How do you price — flat fee, hourly, retainer, commission, something else? Do you take a deposit or require payment upfront? Are stages billed separately? Anything unusual about how you structure payment?"

**Q9 — The dream outcome**
"If AI worked perfectly for you by September 24, 2026 — the day after your second training session — what would change about your week?"

### Step 2 — Wrap up

Read the finished file back to them section by section (or as one block if they prefer) and ask if anything needs correcting. Then confirm: "business-brain.md is saved. This is what your three AI employees will run on when we build them at the live session."

---

## Path B — Gap-Check (prep sheet, existing file, or voice memo transcript)

Use this when a completed or partially completed Business Brain Prep Sheet (Word doc, pasted text, an existing `business-brain.md`, or a voice memo transcript) is available.

1. Read the whole thing first.
2. Map every answer onto the template below, section by section. **If the input is a spoken transcript rather than a structured Prep Sheet:** it likely won't follow the question order, may answer two questions in one breath or drift off-topic — read the whole thing before mapping anything, and use judgment about which section a given passage actually belongs to. Note in the file where you inferred an answer from context rather than a direct response to that exact question.
3. Flag anything **thin or missing**: a one-word answer to a question that needs specifics (e.g., "who's NOT a fit" answered as "difficult people" — too vague to act on), a skipped question, a question the transcript never actually addressed, or an answer that contradicts another section.
4. Ask ONLY about the thin/missing items, one at a time, the same way as Path A. Don't re-ask anything that's already solid — that wastes the time you're trying to save by having a prep sheet or transcript in the first place.
5. Write every clarified answer into `business-brain.md` as you go.
6. When done, tell them plainly which sections you gap-checked and which you left as-is because they were already solid.

If the prep sheet or transcript is empty, barely started, or too rambling to map with confidence, tell them honestly it's not enough to gap-check and offer to just run Path A instead.

---

## Output file structure

Save to `business-brain.md`. Use this structure exactly (headers may stay even if you're mid-interview and a section is still empty — fill in `[not yet answered]` rather than deleting the header):

```markdown
# Business Brain — {{BUSINESS_NAME}}

## Business Basics
- **Name:** {{name}}
- **Role:** {{role}}
- **Business name:** {{business_name}}
- **Industry/niche:** {{industry}}
- **Business size:** {{size}}

## Q1 — Services & Scope
{{answer}}

## Q2 — Ideal Client & Result
{{answer}}

## Q3 — Communication Style
**Tone/phrases/sign-offs:** {{notes}}
**Example lines:** {{1-2 short examples in their voice}}
**Anti-AI Kill List (edited for this business):**
{{their edited list}}

## Q4 — Client Journey
{{answer}}

## Q5 — Recurring Communications
{{answer}}

## Q6 — Team & Tools
{{answer}}

## Q7 — AI Boundaries & Escalation
{{answer}}

## Q8 — Pricing Structure
{{answer}}

## Q9 — The Dream Outcome
{{answer}}
```

---

## Starter Anti-AI Kill List (paste this for Q3)

```
BANNED OPENERS
- "Great question!" / "Absolutely!" / "Certainly!"
- "I'd be happy to help with that."
- "Let's dive into..."
- "In today's fast-paced world..."

BANNED FILLER
- "It's worth noting that..." / "It's important to mention..."
- "At the end of the day..." / "That said..." / "In essence..."

BANNED CORPORATE-SPEAK
- "Leverage" (as a verb), "synergize," "deep dive," "circle back,"
  "touch base," "move the needle," "unlock value," "empower,"
  "game-changer," "holistic," "robust solution"

BANNED STRUCTURAL TELLS
- Three-item bulleted lists dressed up as prose
- "First... Second... Third..." when items aren't sequential
- Closing with "I hope this helps! Let me know if you have any questions."
- Opening with an em-dash

BANNED TONE TELLS
- Flattering the reader in the first sentence ("You're absolutely right to ask...")
- Over-qualifying ("This is just my opinion, but...")
- Over-explaining a simple word choice
```

Golden rule, always: if the person's actual voice conflicts with this list on a specific phrase, their voice wins. This list is a floor, not a ceiling.

## Hard rules for this skill

- Never invent an answer on the person's behalf. If something's unclear, ask — don't guess and write it down as fact.
- Never skip straight to Path B logic without confirming a prep sheet actually exists.
- Always write to file after each answer, not at the end.
- Always flag, out loud, any answer that seems to contradict an earlier one in the same file (e.g., Q2 says "no high-maintenance clients" but Q6 says the person allows unlimited text access).
