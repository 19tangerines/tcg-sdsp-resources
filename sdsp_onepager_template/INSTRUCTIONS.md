# SDSP One-Pager Email Template — Plug-and-Play Guide

This is a reusable email template for SDSP welcome / community-intro emails,
designed to go out to new subscribers (or anyone you want to (re-)introduce
SDSP to). The visual design matches the SDSP brand established in the workshop
template.

**Most of this template is stable** — the welcome paragraph, closing, social
row, and footer don't change per send. The only true fill-in section is the
event cards (block 04 / 05). For most sends you'll only touch the event cards.

To use it:

1. Open each `.html` file in any text editor.
2. Find every `{{PLACEHOLDER}}` and replace it with your content.
3. Copy the file's contents and paste into an Emma **HTML block** in the order
   below.

**Tip:** Use your editor's Find & Replace (`Ctrl+H` on Windows, `Cmd+H` on Mac)
to swap placeholders quickly.

---

## How to assemble in Emma's drag-and-drop editor

Emma uses **rows** (with 1-4 columns) and **content blocks** that you drop into
columns. You'll add rows top-to-bottom in this order:

| # | Row layout | What goes in it |
|---|---|---|
| 1 | 1-column | **Image block** (upload full SDSP logo with tagline, ~327px) then **HTML block** with `01_header_title.html` |
| 2 | 1-column | **HTML block** with `02_welcome_paragraph.html` *(stable boilerplate — rarely edited)* |
| 3 | 1-column | **Divider block** (native Emma block, light grey) |
| 4 | 1-column | **HTML block** with `03_upcoming_events_heading.html` |
| 5–7 | **2-column** ×1–3 | Event cards (see "Event card alternation" below) |
| 8 | 1-column | **Divider block** |
| 9 | 1-column | **HTML block** with `06_closing_paragraph.html` *(stable boilerplate — rarely edited)* |
| 10 | 1-column | **Divider block** |
| 11 | 1-column | **HTML block** with `07_share_button.html` |
| 12 | **4-column**, background `#feba18` | One **Image block** per column: Facebook, Instagram, X, Website icons (64px each, linked) |
| 13 | **2-column** | Left: **Image block** (SDSP logo, 230px). Right: **Image block** (UCSD logo, 230px) |
| 14 | 1-column | **HTML block** with `08_footer.html` |

**Divider block note:** reccomend using the built-in dividers in Emma, but there is a simple grey line divider found in `optional_divider.html` if needed.

---

## ⭐ Event card alternation — IMPORTANT

The "Upcoming Events" section can show **1, 2, or 3 event cards maximum.**
More than 3 starts to feel like a digest, not a welcome — and dilutes each
event. If SDSP has more than 3 events to feature, pick the 3 most relevant
to new subscribers and link to the website for the rest.

**Each card is its own 2-column row.** Alternate the orientation as you go
down for visual rhythm — text-then-image, then image-then-text, then text-then-image
again. Use these files:

- `04_event_card_left.html`  → text in **left** column, image in **right** column
- `05_event_card_right.html` → image in **left** column, text in **right** column

| Number of events | Order |
|---|---|
| 1 event  | `04_event_card_left.html` only |
| 2 events | `04_event_card_left.html`, then `05_event_card_right.html` |
| 3 events | `04_event_card_left.html`, then `05_event_card_right.html`, then `04_event_card_left.html` |

Each event card needs a 2-column row in Emma. Drop the text-side HTML into one
column and a **native Image block** into the other (matching the orientation).
For each event, you're filling in: title, ~30-word blurb, date, the More
Details URL (in the HTML), and uploading one event image (in the Image block).

---

## Image uploads

For every Image block, upload the PNG directly to Emma's image library when
you add the block. Emma will host the image on their CDN automatically — no
need to host elsewhere.

Images you'll need:
- **Full SDSP logo with tagline** (~327px, row 1) — use the full version that
  includes "Community, Learning, and Research"
- One image per event card (~250px wide, row 5–7) — workshop topic illustration,
  flyer crop, photo, etc.
- Facebook / Instagram / X / Website icons (row 12, 64px each)
- **SDSP logo** (~230px, row 13) — can be the simpler logo here, not the
  full-tagline version
- UCSD logo (~230px, row 13)

---

## Brand reference

Same palette and fonts as the workshop template (deliberate brand cohesion):

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
| `01_header_title.html` | `{{HEADLINE}}` — recommended: **"Welcome to the San Diego Science Project"** (simple, evergreen, doesn't fight the paragraph's "Hi there!" hook). See title options section below for alternatives. |
| `02_welcome_paragraph.html` | `{{SDSP_WEBSITE_URL}}` *(set once)* — stable boilerplate otherwise. Describes SDSP's partnership with UC San Diego and the SD County Office of Education, the California Science Project network, and research partners like Scripps and Birch Aquarium. |
| `03_upcoming_events_heading.html` | *(no edits — says "Upcoming Events")* |
| `04_event_card_left.html` | `{{EVENT_TITLE}}`, `{{EVENT_BLURB}}`, `{{EVENT_DATE}}`, `{{MORE_DETAILS_URL}}` (URL appears 2x — use Find & Replace) |
| `05_event_card_right.html` | Same placeholders as 04 |
| `06_closing_paragraph.html` | `{{SDSP_EVENTS_URL}}` *(set once)* — stable boilerplate otherwise. Includes a call-to-action encouraging readers to refresh their practice, connect with the community, and explore upcoming workshops at sdscienceproject.org. |
| `07_share_button.html` | `{{SHARE_URL}}` (appears 2x — use Find & Replace) |
| `08_footer.html` | `{{YEAR}}` — current year for copyright; unsubscribe + mailing address use Emma's standard merge tags |

---

## Workshop topics — suggested event blurbs

SDSP workshops span a range of timely, relevant topics. Use these as starting
points for `{{EVENT_BLURB}}` when filling in event cards. Each is ~30 words —
adapt as needed for a specific workshop within the topic.

| Topic | Suggested blurb |
|---|---|
| **Science Media Literacy** | Help students evaluate scientific claims, spot misinformation, and think critically about the science they encounter in the real world. |
| **Climate Education** | Connect with UC San Diego researchers and explore place-based, phenomenon-driven approaches to teaching climate science, from local coastlines to global systems. |
| **AI & Science Communication** | Examine how artificial intelligence is reshaping the way science is produced and communicated — and what that means for your classroom. |
| **NGSS & Assessment Design** | Expand your skills for designing equitable, student-centered assessments aligned to the Next Generation Science Standards. |

These topics aren't exhaustive — SDSP workshops also cover emerging areas as
they come up. If your event doesn't fit one of these, write a ~30-word blurb
in the same style: what the workshop is about, who it helps, and what teachers
take away.

---

## Title options

The "San Diego Science Project: ___" pattern matches the workshop template
("Series: Workshop @ Location"), but for the one-pager you can also drop the
colon altogether since this email is about identity, not an event. Some options
in order of recommendation:

1. **Welcome to the San Diego Science Project** *(recommended)* — simple,
   evergreen, sets up the "Hi there, it's nice to meet you!" intro without
   competing with it.
2. **San Diego Science Project: Welcome to the community** — keeps the
   colon pattern from the workshop template for brand cohesion.
3. **San Diego Science Project: Community, Learning, and Research** — uses
   their actual tagline. More institutional, less warm.
4. **Meet the San Diego Science Project** — slight twist, inviting tone.

Pick whichever fits the audience. Option 1 is the safest evergreen choice.

---

## Preview

Open `assembled_preview.html` in any web browser to see what the final email looks like with sample images filled in. Use it as a visual reference.
