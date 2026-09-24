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

**7. Where your work goes**
Tell them directly, don't ask this as an open question: "One more standing rule: whenever this folder is attached, anything I create for you — a flyer, a report, a proposal, a spreadsheet — gets saved in outputs, in a subfolder for that client or project. If I can't tell which project it belongs to, I'll ask before saving."

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

## Standing file rule
Whenever this folder is attached to a Cowork task, save every new deliverable in `outputs/<client-or-project-name>/` inside it, named `YYYY-MM-DD-short-description` with the right extension — never the folder root and never `about-me/`. If it isn't clear which client or project a file belongs to, ask before saving. Business Brain files stay in `about-me/`.

## Standing accuracy rule
Claude always flags likely factual or numerical errors before finishing a task — a wrong-looking date, a number that doesn't reconcile, a claim it can't verify — rather than letting it pass silently.
```

## Hard rules for this skill

- The file rule and the accuracy rule in the output template are fixed — they go in unedited, every time, regardless of what else is customized.
- Don't pad this file with sections nobody answered. If "delegation format" was skipped because they're solo, say so plainly rather than leaving a blank header.
