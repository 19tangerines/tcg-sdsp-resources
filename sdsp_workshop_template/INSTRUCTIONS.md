# SDSP Workshop Email Template — Plug-and-Play Guide

This is a reusable email template for SDSP workshop announcements. The visual design matches past SDSP workshop emails. To use it for a new workshop, you'll:

1. Open each `.html` file in any text editor (Notepad, TextEdit, VS Code, even Google Docs in plain-text mode).
2. Find every `{{PLACEHOLDER}}` and replace it with your workshop's content.
3. Copy the file's contents and paste into an Emma **HTML block** in the order below.

**Tip:** Use your editor's Find & Replace (`Ctrl+H` on Windows, `Cmd+H` on Mac) to swap placeholders quickly.

---

## How to assemble in Emma's drag-and-drop editor

Emma uses **rows** (with 1-4 columns) and **content blocks** that you drop into columns. You'll add rows top-to-bottom in this order:

| # | Row layout | What goes in it |
|---|---|---|
| 1 | 1-column | **Image block** (upload SDSP logo, ~327px) then **HTML block** with `01_header_title.html` |
| 2 | 1-column | **HTML block** with `02_intro_paragraph.html` |
| 3 | 1-column | **Divider block** (native Emma block, light grey) |
| 4 | 1-column | **HTML block** with `03_workshop_heading.html` |
| 5 | 1-column | **HTML block** with `04_workshop_description.html` |
| 6 | 1-column | **HTML block** with `05_workshop_outcomes_list.html` |
| 7 | 1-column | **HTML block** with `06_workshop_takeaway.html` |
| 8 | 1-column | **Divider block** |
| 9 | 1-column | **HTML block** with `07_event_details_heading.html` |
| 10 | **2-column** | Left: **HTML block** with `08_event_details_left.html`. Right: **Image block** (upload workshop topic image, ~250px) |
| 11 | 1-column | **HTML block** with `09_register_button.html` |
| 12 | 1-column | **Divider block** |
| 13 | 1-column | **HTML block** with `10_about_sdsp.html` *(stable boilerplate — no edits needed)* |
| 14 | 1-column | **Divider block** |
| 15 | 1-column | **Image block** (upload workshop flyer, ~500px, link it to the registration page) |
| 16 | 1-column | **Divider block** |
| 17 | 1-column | **HTML block** with `11_share_button.html` |
| 18 | **4-column**, background `#feba18` | One **Image block** per column: Facebook, Instagram, X, Website icons (64px each, linked to your social pages) |
| 19 | **2-column** | Left: **Image block** (SDSP logo, 230px). Right: **Image block** (UCSD logo, 230px) |
| 20 | 1-column | **HTML block** with `12_footer.html` |

**Total row width:** target 500px (Emma's default content width works fine).

**Divider block note:** reccomend using the built-in dividers in Emma, but there is a simple grey line divider found in `optional_divider.html` if needed.

---

## Image uploads

For every Image block, upload the PNG directly to Emma's image library when you add the block. Emma will host the image on their CDN automatically — no need to host elsewhere.

Images you'll need:
- SDSP logo (used in row 1 and row 19)
- Workshop topic image (row 10, optional but recommended)
- Workshop flyer (row 15, optional)
- Facebook / Instagram / X / Website icons (row 18)
- UCSD logo (row 19)

---

## Brand reference

These are the colors and fonts baked into the template:

- Headings (navy): `#182b49`
- Body text (grey): `#444a5b`
- Footer text (near-black): `#101112`
- Button / accent (light blue): `#3aaee0`
- Social row background (yellow): `#feba18`
- Font: Arial, Helvetica, sans-serif

---

## What to fill in (cheat sheet)

| File | Placeholders |
|---|---|
| `01_header_title.html` | `{{HEADLINE}}` — e.g. "Summer Professional Learning Events: Science Media Literacy Workshop @ UC San Diego" |
| `02_intro_paragraph.html` | `{{INTRO_HOOK}}`, `{{WORKSHOP_OFFERING_SENTENCE}}` |
| `03_workshop_heading.html` | `{{WORKSHOP_NAME}}` |
| `04_workshop_description.html` | `{{WORKSHOP_DESCRIPTION}}` |
| `05_workshop_outcomes_list.html` | `{{OUTCOME_1}}`, `{{OUTCOME_2}}`, `{{OUTCOME_3}}` (add more `<li>` lines if needed) |
| `06_workshop_takeaway.html` | `{{TAKEAWAY_SENTENCE}}` |
| `07_event_details_heading.html` | *(no edits — says "Event Details")* |
| `08_event_details_left.html` | `{{DATE}}`, `{{TIME}}`, `{{LOCATION}}`, `{{AUDIENCE}}`, `{{COST}}` |
| `09_register_button.html` | `{{REGISTRATION_URL}}` (appears 2x — use Find & Replace) |
| `10_about_sdsp.html` | `{{SDSP_WEBSITE_URL}}` *(set once, then leave this file alone)* |
| `11_share_button.html` | `{{SHARE_URL}}` (appears 2x — use Find & Replace) |
| `12_footer.html` | `{{YEAR}}` — current year for copyright line; unsubscribe + mailing address use Emma's standard merge tags |

---

## Preview

Open `assembled_preview.html` in any web browser to see what the final email looks like with the original Science Media Literacy Workshop content filled in. Use it as a visual reference.
