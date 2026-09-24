---
name: brand-kit-builder
description: Builds brand-kit.md and stores the business's actual letterhead file, so every AI employee that drafts correspondence or agreements uses the real brand colors, fonts, and letterhead instead of guessing. New module, not part of the original attorney kit. ~10 minutes. Trigger on "brand kit," "my brand," "letterhead," "brand colors," or any request to build or fill out a brand file.
---

# Brand Kit Builder

`business-brain.md` is the business mechanics. `writing-rules.md` is the voice. `about-me.md` is the person. This file is the **visual identity** — colors, fonts, logo, letterhead — so anything an AI employee drafts (an agreement, a letter, an invoice) actually looks like it came from this business instead of a generic template.

Not required, but strongly recommended for anyone whose Intake Coordinator or Email Manager will be drafting documents that go out under the business's name.

Budget about 10 minutes.

## Before anything else — confirm the folder

Everything this training builds lives in one folder the person attached to this Cowork task, so their AI employees can find it later.

1. Check whether a folder is attached to this task. If none is, stop and say: "Before we start, attach the folder where you want your Business Brain files to live (for example, a folder named My Business Brain). Tell me when it's attached." Don't ask any interview questions until a folder is attached.
2. Confirm out loud before writing anything: "I'll save your files in [folder name]/about-me/. Sound good?" Create `about-me/` if it doesn't exist yet.
3. Save every file this skill creates in that `about-me/` folder, including any letterhead and logo files they upload — never the folder root, a temporary location, or anywhere else. If the person asks for a different location, use it, and tell them plainly that their AI employees look in `about-me/` by default.

## How to run it

One question at a time. Save to `about-me/brand-kit.md` as you go. If a letterhead file gets uploaded, save the actual file too (see Output below) — the .md file describes the brand, it doesn't replace the real letterhead document.

Ask, in order:

**1. Letterhead — do you already have one?**
"Do you have an existing letterhead template — a Word doc, PDF, or Canva/Google Doc export you already use for official documents? If so, upload it now. If not, that's fine — say so and we'll build the header from your brand basics instead."

If uploaded: confirm the file type and save it (see Output). You can pull colors, fonts, and header layout straight from the document itself rather than re-asking questions 3-6 — only ask those if something's genuinely missing from the file (e.g., it has a logo but no clear hex colors).

If not uploaded, continue through the rest in order.

**2. Multiple letterheads or brands?**
"Do you operate under more than one name or brand — different divisions, a DBA, separate letterheads for different services? If so, list each one and whether it needs its own letterhead, or if they all share this one."

Note this even if they said yes to Question 1 — a business can have a primary letterhead and one or more secondary ones.

**3. Legal name vs. everyday name**
"What's the exact legal/registered name that has to appear on official documents — the one on your license, LLC filing, or registration? Is that the same as the name you go by day to day, or different (e.g., 'McPherson Law' vs. 'McPherson Law Offices LLC')? I'll use the exact legal name on formal documents and the everyday name elsewhere, unless you tell me otherwise."

**4. Logo**
"Do you have a logo file (PNG, JPG, or SVG)? Upload it if so. If not, no problem — we'll use your business name in text instead."

**5. Brand colors**
"What are your brand colors? Hex codes if you know them (like #6E1423) are ideal, but 'burgundy and gold' or 'navy and white' works fine too — I'll match the closest hex values."

**6. Fonts**
"Do you have specific fonts you use for headings and body text? If you're not sure, say so — I'll use a clean, professional default."

**7. Header info for documents**
"What should appear in the header of an official document — business name, address, phone, email, website? Give me exactly what you want shown, in the order you want it."

**8. Signature block**
"When a document is signed on your behalf, what should the signature block show — your name, title, credentials, license/bar number if applicable, company name? Give me it exactly as it should appear."

**9. Required footer or disclaimer text**
"Is there anything that legally or professionally has to appear on your documents — a licensing disclosure, a confidentiality notice, a regulatory line, an E&O/malpractice notice? This is different from a tagline — it's language you're required or expected to include, not marketing. Skip if nothing applies."

**10. Preferred file format**
"When a document is finished, do you want it delivered as a Word doc, a PDF, or both? And do you have a preference for how it's named (a naming convention you already use)?"

**11. Tagline or slogan — optional**
"Do you use a tagline or slogan on official documents? Skip if not."

**12. Anything else brand-specific**
"Anything else — a specific way your business name must always be written (capitalization, 'LLC' always included, trademark symbol, etc.), colors or styles to avoid, an old logo version that should never be used? Skip if nothing comes to mind."

## Output

**1. Save the actual letterhead/logo files, if provided**, in `about-me/` alongside `brand-kit.md` (not just described in the text) — these are what actually get used when drafting, the .md file is the index.

**2. Save `about-me/brand-kit.md`:**

```markdown
# Brand Kit — {{BUSINESS_NAME}}

## Letterhead(s)
{{"On file: [filename] — use this as the base for all drafted documents." OR "No letterhead on file — build headers from the brand basics below."}}
{{If multiple: list each brand/division, its filename (or "no letterhead — use shared basics"), and when to use which.}}

## Legal name vs. everyday name
- **Legal/registered name (use on formal documents):** {{exact legal name}}
- **Everyday name (use elsewhere):** {{everyday name, or "same as legal name"}}

## Logo
{{"On file: [filename]" OR "No logo on file — use business name in text."}}

## Brand colors
- **Primary:** {{name/description}} — {{hex if known}}
- **Secondary:** {{name/description}} — {{hex if known}}
- **Accent:** {{name/description}} — {{hex if known, or "not specified"}}

## Fonts
- **Headings:** {{font or "not specified — use a clean professional default"}}
- **Body:** {{font or "not specified — use a clean professional default"}}

## Document header
{{exactly what they specified, in their order}}

## Signature block
{{exactly as specified — name, title, credentials, license/bar number, company}}

## Required footer / disclaimer text
{{exact required language, or "None specified"}}

## File format & naming
- **Preferred format:** {{Word / PDF / both}}
- **Naming convention:** {{if given, or "Not specified — use YYYY-MM-DD-description as default"}}

## Tagline
{{tagline, or "None"}}

## Other brand rules
{{list — required wording, things to avoid, old assets never to use — or "None specified"}}
```

## How other AI employees use this

Any skill that drafts a document under this business's name — Intake Coordinator drafting an agreement, Email Manager drafting correspondence — checks for `brand-kit.md` and the letterhead file first:

1. **Letterhead on file** → draft on it directly. If more than one is on file, match the right one to the brand/division the document is for.
2. **No letterhead, but colors/fonts/header specified** → build a clean header from those specifics, using the legal name on formal documents and the everyday name elsewhere, per the brand-kit.
3. **`brand-kit.md` doesn't exist at all** → fall back to business name and business address from `business-brain.md`. Never invent colors, a logo, a letterhead, or a required disclaimer that wasn't provided.

Required footer/disclaimer language and the signature block are not optional flourishes — include them on every document brand-kit.md says they belong on, the same way a hard rule gets followed, not treated as a style preference to skip under time pressure.

## Hard rules for this skill

- Never invent a hex color, a font, a legal name, a signature block, a required disclaimer, or letterhead content that wasn't given. "Not specified" is a valid, honest answer — guessing at what looks "professional enough" is not.
- Never redraw or recreate a logo from a description — only use an actual uploaded logo file. A described logo with no file gets "no logo on file," not an invented one.
- If a letterhead file is uploaded, save the real file — don't just transcribe what it looks like into markdown. Other skills need the actual document to draft on.
- If there's more than one letterhead/brand, never guess which one applies to a given document — ask, unless the business/service type makes it unambiguous from context already captured in business-brain.md.
