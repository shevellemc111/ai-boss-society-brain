---
name: how-i-work-builder
description: Optional. Builds how-i-work.md — standing rules for how Claude should operate day to day with this person, separate from what the business does. Use anytime after about-me.md and business-brain.md exist. Trigger on "how I work," "how i work file," "set up how Claude works with me," or any request to define working preferences or standing rules.
---

# How I Work Builder

This is **optional** — unlike Business Brain, Writing Rules, and About-Me. It's worth doing if someone wants more control over Claude's default behavior, but nobody should feel behind for skipping it.

Budget about 10 minutes if they choose to do it.

## Before anything else — confirm the folder

Everything this training builds lives in one folder the person attached to this Cowork task, so their AI employees can find it later.

1. Check whether a folder is attached to this task. If none is, stop and say: "Before we start, attach the folder where you want your Business Brain files to live (for example, a folder named My Business Brain). Tell me when it's attached." Don't ask any interview questions until a folder is attached.
2. Confirm out loud before writing anything: "I'll save your files in [folder name]/about-me/. Sound good?" Create `about-me/` if it doesn't exist yet.
3. Save every file this skill creates in that `about-me/` folder — never the folder root, a temporary location, or anywhere else. If the person asks for a different location, use it, and tell them plainly that their AI employees look in `about-me/` by default.

## Pre-work answers: check first

Before asking anything, look in `about-me/prework/` for their Pre-Work Packet (Word, PDF, or text) or voice memo transcript. The Business Brain builder saves it there. If nothing is there, ask once: "Did you fill out the Pre-Work Packet or record a voice memo? Upload or paste it here and I'll use what you already answered." If they upload or paste one now, save a copy to `about-me/prework/` (keep the file name; pasted text goes in `about-me/prework/prework-answers.md`) so nothing else has to ask for it again. If one was already there, ask before using it: "I found your pre-work ([file name]). Want me to use it and only ask about what's missing, or would you rather answer the questions fresh?" Go with what they choose.

**If they want to use their pre-work:**
1. Read the whole thing first and find the **8. How I Work** section. A voice memo transcript won't follow the question order, so map each passage to the question it actually answers.
2. Fill in every question the pre-work answers clearly, writing to the file as you go.
3. Tell them: "Your pre-work fully answered [x] of 5 questions. I just need you on: [short list]." If it covered everything, say so and go straight to reading the file back for confirmation.
4. Ask only about the gaps, **one at a time**. A gap is:
   - a question that was skipped or never came up in the transcript
   - a question only partly answered (ask just for the missing part)
   - an answer too vague to act on (for example, "difficult people" for a red flag, or "sometimes" for a schedule)
   - an answer that contradicts the Business Brain or another answer
   - anything you're not sure you understood

   Never guess to fill a gap, and don't re-ask anything the pre-work already answers clearly. If you filled something by reading between the lines rather than from a direct answer, mark it `(inferred, please confirm)` and check it with them when you read the file back.

**Switching midway:** if they're answering the questions fresh (or said they had no pre-work) and then say something like "just use my pre-work," switch right away. Keep everything they've already answered here (their newest answers win over the pre-work), fill in the rest from the pre-work (ask them to upload it if it isn't in `about-me/prework/` yet), tell them what's left ("Between what you've answered here and your pre-work, [x] of [total] are done. I just need you on: [short list]."), and ask only the gap questions. It works the other way too: if they'd rather answer the rest fresh, go back to the regular questions for whatever's left. While they're answering fresh, don't pull answers from the pre-work.

**If there's no pre-work, or they'd rather answer fresh,** run the questions below as usual.

## How to run it

One question at a time, write to file as you go. This is short enough that it rarely needs a gap-check path — if someone has partial answers already, just ask about what's missing.

**1. Response length**
"When you ask me something, do you usually want the short answer, or the fuller explanation with reasoning? Does that change depending on what you're asking about?"

**2. Ask-first vs. proceed**
"For routine tasks — drafting something, organizing files, pulling together info — should I just do it and show you the result, or check in with you first before starting? Does that answer change for anything higher-stakes, like something going out to a client?"

**3. Options vs. single pick**
"When there's more than one reasonable way to do something, do you want me to just make a call and tell you what I picked, or lay out the options and let you choose?"

**4. Default file format**
"When I create something for you, what's the default format you want — a doc, a plain message in chat, a spreadsheet, something else? Does it depend on what the deliverable is?"

**5. Delegation format (skip if solo)**
"If you have a team or contractors, how do you want me to hand off work to them — a written brief, a task in whatever tool you use, something else? If it's just you, skip this one."

**6. Accuracy check**
Tell them directly, don't ask this as an open question: "One standing rule that's always on, no matter what you answer above: I always flag anything that looks like a likely factual or numerical error before finishing — a wrong-looking date, a number that doesn't add up, a claim I can't verify. I'll say so plainly rather than let it slide through."

## Output file structure

Save to `about-me/how-i-work.md`:

```markdown
# How I Work With Claude — {{NAME}}

## Response length
{{answer}}

## Ask-first vs. proceed
{{answer, noting any distinction between routine and higher-stakes tasks}}

## Options vs. single pick
{{answer}}

## Default file format
{{answer}}

## Delegation format
{{answer, or "Solo — not applicable."}}

## Standing accuracy rule
Claude always flags likely factual or numerical errors before finishing a task — a wrong-looking date, a number that doesn't reconcile, a claim it can't verify — rather than letting it pass silently.
```

## Hard rules for this skill

- The accuracy rule in the output template is fixed — it goes in unedited, every time, regardless of what else is customized.
- Don't pad this file with sections nobody answered. If "delegation format" was skipped because they're solo, say so plainly rather than leaving a blank header.
