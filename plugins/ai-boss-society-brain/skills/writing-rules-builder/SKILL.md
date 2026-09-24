---
name: writing-rules-builder
description: Required. Builds writing-rules.md from three real writing samples across different registers, so AI-drafted content actually sounds like the person. Use after business-brain.md exists (or alongside it). Trigger on "writing rules," "my writing samples," "voice module," "writing rules pre-work," or any request to build writing rules or capture voice/writing samples.
---

# Writing Rules Builder

Q3 in the Business Brain module is a quick snapshot: a described tone, a couple of example lines, an edited kill list — no full sample. This skill is the deep version — it collects real writing across three different registers and hands back a voice profile the person confirms or corrects, instead of working from a described tone alone.

This module is **required** for everyone in this training, unlike the attorney version of this kit where it was optional. Voice work carries more weight here — this group skews toward coaches and other personal-brand businesses where the writing has to sound like a specific human, not just be professionally correct.

Budget 20-25 minutes.

## Step 1 — Collect three samples, one per register

Ask for three writing samples, explicitly across these three registers — not three examples of the same kind of writing:

1. **Client/customer-facing** — a real email, letter, or proposal sent to an actual client or prospect.
2. **Social** — a real social media post (any platform).
3. **Transcript / spoken-to-written** — a voice memo transcript, a video caption, a webinar chat message, anything that started as spoken words and got written down. This one matters because it usually reveals rhythm and word choice that polished writing hides.

Accept samples pasted directly, uploaded as files, or described and then pasted. Take what's actually offered — don't demand all three be perfect or lengthy; a short but real sample beats a long invented one.

**Already have a voice memo transcript from Business Brain or About Me?** That covers the transcript/spoken register — don't make them record a second one. Pull it in here and just collect the client-facing and social samples fresh.

### If they don't have samples ready

Don't block. Offer, in order:

1. "Pull one up on your phone right now — a text to a client, an old Instagram caption, anything real. Paste it here." This is the fastest fix and covers most people.
2. If that's still not possible for a given register, get a short live sample instead: ask them to write two or three sentences right now as if they were actually sending it (e.g., "text me like you're telling a client their project's done a day late"). A live sample beats no sample.
3. Only skip a register entirely if both of those fail, and say plainly in the output that register wasn't covered and drafts in that register should be treated as unverified until a real sample is added later.

## Step 2 — Analyze, don't guess

Read all three samples together and look for real, repeatable patterns — not vibes. Specifically:

- **Sentence rhythm** — average sentence length, whether they favor short punchy sentences or longer ones, fragments, run-ons, how they use punctuation (dashes, ellipses, exclamation points).
- **Vocabulary** — words and phrases that show up more than once, words that feel distinctly "them," any jargon or industry shorthand they use naturally.
- **Structure** — paragraph length, whether they use bullets/lists naturally or write in blocks, how they open and close a piece of writing, whether headers show up at all.
- **Recurring phrases** — actual repeated phrases or verbal tics across the samples (a signature sign-off, a phrase they lean on to soften bad news, a way they open every post).
- **How it shifts by register** — what changes between client-facing, social, and transcript. Most people are noticeably more formal client-facing and looser on social; the transcript sample usually shows the rawest, truest rhythm. Name the specific differences, don't just say "more casual on social."

## Step 3 — Present findings for confirmation, not as a final answer

Show your analysis back to them in plain language, organized as:

- **Overall voice** — 3-5 sentences describing how they write across contexts, using specifics from their actual samples, not generic adjectives.
- **By register:**
  - Client-facing: {{specific observations}}
  - Social: {{specific observations}}
  - Casual/transcript: {{specific observations}}
- **Recurring phrases/vocabulary found**
- **Anything surprising or worth flagging** (e.g., "your client emails and your social posts read like two different people — is that intentional, or should one shift toward the other?")

Ask directly: "Does this sound like you? Anything wrong, missing, or that you'd word differently?" Iterate on their corrections before finalizing. Never treat your first-pass analysis as done without this check — the whole point of this module is accuracy over a guess.

## Step 4 — Reconcile with the Business Brain Q3 kill list

If `business-brain.md` already has a Q3 Anti-AI Kill List, pull it in as-is — don't rebuild it from scratch. Note explicitly in the output: "This file goes deeper than the Business Brain Q3 snapshot. The kill list from Q3 still applies — see business-brain.md — this file adds the register-specific voice detail Q3 doesn't cover."

If `business-brain.md` doesn't exist yet or Q3 hasn't been done, use the same Starter Anti-AI Kill List from the business-brain-builder skill and let them edit it here instead, then note it should also get copied into business-brain.md's Q3 when that module runs.

## Output file structure

Save to `writing-rules.md`:

```markdown
# Writing Rules — {{BUSINESS_NAME}}

## Overall voice
{{3-5 sentence summary, specific to this person}}

## By register

### Client/customer-facing
{{observations + 1 illustrative line pulled from their own sample}}

### Social
{{observations + 1 illustrative line pulled from their own sample}}

### Transcript / casual spoken
{{observations + 1 illustrative line pulled from their own sample}}

## Vocabulary & recurring phrases
- **Words/phrases they reach for:** {{list}}
- **Words/phrases they'd never use:** {{list, if known}}

## Structural habits
- Paragraph length: {{}}
- Bullets vs. prose: {{}}
- Openers/closers: {{}}

## Anti-AI Kill List
(Pulled from business-brain.md Q3 if it exists — otherwise built here and flagged for copy-back.)
{{list}}

## When breaking the rules is OK
- When they're deliberately being playful, silly, or self-deprecating — match that tone.
- When a technical/industry term is the correct word — use it plainly, don't dress it up.
- When it's a real announcement, not hype — a direct, plain headline is fine.

**Golden rule:** if this person's actual voice conflicts with the kill list on a specific phrase, their voice wins. The kill list is a floor, not a ceiling.

## Coverage note
{{Which of the 3 registers had a real sample vs. a live/substitute sample vs. was skipped — be honest here so future drafts in an unverified register get extra review.}}
```

## Hard rules for this skill

- Never fabricate a writing sample or fill in a register with invented text. If a register wasn't covered, say so in the Coverage note — don't paper over the gap.
- Always show the analysis back for confirmation before saving as final. Skipping this step is exactly the kind of thing that leads to a voice profile that doesn't actually sound like the person.
- Don't overwrite an existing Q3 kill list in business-brain.md from here — read it in, don't replace it, unless the person explicitly asks to redo it.
