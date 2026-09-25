---
name: about-me-builder
description: Required. Builds about-me.md — who the person is as an operator, separate from how their business runs. New module, not part of the original attorney kit. ~15 minutes. Trigger on "about me," "my about-me file," "about me pre-work," or any request to build or fill out an about-me file.
---

# About-Me Builder

`business-brain.md` is about the business — services, clients, pricing, process. This file is about the **person running it**: how they think, what they're juggling, how they learn, and what's made AI actually useful for them before. Claude reads this alongside `business-brain.md`, but it's a separate file and a separate section of the interview — don't merge them.

Required. Budget about 15 minutes.

## Before anything else — confirm the folder

Everything this training builds lives in one folder the person attached to this Cowork task, so their AI employees can find it later.

1. Check whether a folder is attached to this task. If none is, stop and say: "Before we start, attach the folder where you want your Business Brain files to live (for example, a folder named My Business Brain). Tell me when it's attached." Don't ask any interview questions until a folder is attached.
2. Confirm out loud before writing anything: "I'll save your files in [folder name]/about-me/. Sound good?" Create `about-me/` if it doesn't exist yet.
3. Save every file this skill creates in that `about-me/` folder — never the folder root, a temporary location, or anywhere else. If the person asks for a different location, use it, and tell them plainly that their AI employees look in `about-me/` by default.

## Pre-work answers: check first

Before asking anything, look in `about-me/prework/` for their Pre-Work Packet (Word, PDF, or text) or voice memo transcript. The Business Brain builder saves it there. If nothing is there, ask once: "Did you fill out the Pre-Work Packet or record a voice memo? Upload or paste it here and I'll use what you already answered." If they upload or paste one now, save a copy to `about-me/prework/` (keep the file name; pasted text goes in `about-me/prework/prework-answers.md`) so nothing else has to ask for it again.

**If pre-work answers exist:**
1. Read the whole thing first and find the **3. About Me** section. A voice memo transcript won't follow the question order, so map each passage to the question it actually answers.
2. Fill in every question the pre-work answers clearly, writing to the file as you go.
3. Tell them: "Your pre-work fully answered [x] of 9 questions. I just need you on: [short list]." If it covered everything, say so and go straight to reading the file back for confirmation.
4. Ask only about the gaps, **one at a time**. A gap is:
   - a question that was skipped or never came up in the transcript
   - a question only partly answered (ask just for the missing part)
   - an answer too vague to act on (for example, "difficult people" for a red flag, or "sometimes" for a schedule)
   - an answer that contradicts the Business Brain or another answer
   - anything you're not sure you understood

   Never guess to fill a gap, and don't re-ask anything the pre-work already answers clearly. If you filled something by reading between the lines rather than from a direct answer, mark it `(inferred, please confirm)` and check it with them when you read the file back.

**If there are no pre-work answers,** run the questions below as usual.

## How to run it

One question at a time, same as the Business Brain interview. Write each answer to `about-me.md` as you go, don't batch it to the end. If someone already has an `about-me.md` from another tool or a prior session, read it first and gap-check the thin spots instead of starting over — same logic as the Business Brain Prep Sheet path.

**Voice memo option:** offer this up front, same as Business Brain — "If you'd rather talk through this than type it, record yourself out loud answering these 9 questions — your phone's voice memo app is the easiest way, or your computer's dictation/recording tool if that's easier for you — get a text transcript, and upload or paste it here instead." Treat an uploaded transcript the same way as an existing `about-me.md`: read the whole thing first, map what you can onto the 9 sections below (a spoken transcript won't follow the question order — use judgment on where each part belongs), then ask one at a time about anything thin, missing, or unclear from context. Don't re-ask what's already solid.

Ask, in order:

**1. Who you are**
"Your name, your role or title, your business name, and where you're based?"

**2. What you do, dinner-party version**
"If someone at a dinner party asked what you do, what's the one or two sentences you'd actually say — no jargon, no elevator-pitch polish?"

**3. Current roles and ventures**
"What are you actively running right now, and what stage is each one in — just getting started, actively building, fully launched, scaling, or just maintaining? If something's on the back burner, say so and why."

**4. Who you work with**
"Who are your clients or customers, in a sentence? And who else is involved in the business day to day — a team, contractors, a partner, or is it just you?"

**5. Tools**
"What do you open every day? What do you use weekly or monthly but not daily? And is there anything you're supposed to use but actually avoid?"

**6. Personal context — optional**
"This one's optional, skip it if you'd rather not: is there anything personal worth knowing — family, lifestyle, what's driving you right now — that would help Claude understand your context, not just your business? Totally fine to skip or keep this brief."

Do not push if they skip this. Don't ask a follow-up probing for more. One offer, then move on.

**7. How you learn best**
"When you're figuring out something new — a tool, a process, a concept — what actually works for you? Reading it out, watching someone do it, trying it yourself and breaking it, a quick explanation before you dive in?"

**8. What's worked in past AI sessions**
"Think of a time working with Claude or another AI tool went well. What made it work — 2-3 specific things you want to see repeated?"

**9. Anything else**
"Anything else you want Claude to know about you that didn't fit anywhere above?"

## Output file structure

Save to `about-me/about-me.md`:

```markdown
# About Me — {{NAME}}

## Who I am
- **Name:** {{name}}
- **Role:** {{role}}
- **Business:** {{business_name}}
- **Location:** {{location}}

## What I do (plain version)
{{dinner-party description}}

## Current roles & ventures
- **{{venture 1}}** — {{status}}
- **{{venture 2}}** — {{status}}
- **On the back burner:** {{if any}} — {{why}}

## Who I work with
- **Clients/customers:** {{description}}
- **Team:** {{who, or "just me"}}

## Tools
- **Daily:** {{list}}
- **Weekly/monthly:** {{list}}
- **Avoid, even though "supposed to" use:** {{if any}}

## Personal context (optional)
{{whatever was shared, or "Not shared — that's fine."}}

## How I learn best
{{answer}}

## What's made past AI sessions successful
{{answer}}

## Anything else
{{answer, or "Nothing further."}}
```

## Hard rules for this skill

- Never make personal context mandatory. If skipped, write "Not shared — that's fine." and move on — don't leave a placeholder that reads like an unfinished task.
- Keep this file about the person, not the business mechanics — if an answer drifts into pricing, services, or client process, that belongs in `business-brain.md`; note it there instead and keep this file lean.
- Don't guess at tone or add color commentary — this file is a factual reference, not a writing sample (that's what writing-rules.md is for).
