# Executive Essentials — Deck Brief for Claude Code

## What we're building

A 60-minute HTML slide deck for **AI Executive Essentials**, the entry-level offer from Capable AI (capableai.io). Audience: C-suite + senior leadership (CEO, CIO, CFO, COO, GC). Outcome: walk out with the confidence to make AI strategy decisions and a defensible view of what their organisation needs next.

This is a **briefing deck, not a training deck or a sales deck**. The visual language is restrained, executive-grade, and built around two or three slides that land hard.

Adapt the existing `deck.html` template — same fonts, colour system, navigation. **Reuse the CSS wholesale.** Drop the ARIA/APX banking-specific classes (phone mockup, tier-card banking content, anatomy banking content, biz-hero banking numbers). Keep everything else.

Output: a single self-contained `executive-essentials-deck.html` file in the same project root.

---

## The thesis

> Speed to value comes from investing up front in architecture, not from buying licences and hoping.

Plant it in Act 1. Pay it off in every act after.

---

## Anti-AI-deck principles (READ THIS FIRST)

The single biggest risk in this deck is that it ends up looking AI-generated: word-soup slides, three-card rhythm repeating to infinity, generic stat cards, centred everything, no personality. **Fight this on every slide.**

**1. Text density — hard caps.**
- Slide titles: ≤ 8 words.
- Sub-titles: ≤ 12 words.
- Body text per element: ≤ 20 words. Often fewer.
- Some slides have a title and nothing else. Some are a single number. **Most slides should feel under-filled, not over-filled.** White space is the design.

**2. Vary the slide shape.**
- Do not put three-card slides next to each other.
- Intersperse: full-bleed text, single-number slides, asymmetric layouts, pull-quote moments, dark slides used as emotional beats not just dividers.
- Rhythm matters. A reader should feel the deck change tempo.

**3. Break the format twice.**
- There are two slides in this deck (marked below) where you should *deliberately break the template's standard layout* to create a moment. One is the "uncomfortable prompt" slide in the Readiness section. The other is the pull-quote at the start of Rollout. Treat these like a film cut.

**4. No stock images. No AI-generated images. No icon-libraries.**
- Build all visuals from CSS / SVG / type. Hatched grid (already in template), gradient washes, hand-drawn-looking SVG shapes, mono-font ASCII-style diagrams, typographic compositions where the text *is* the visual.
- The Levels diagram is the one place a proper SVG shape is welcome — six labelled nodes on a horizontal line, ascending. Hand-drawn quality.

**5. Personality in the typography.**
- Use the full type system. Mono for chips and labels. Serif italic for emphasis and pull-quotes. Body sans for everything else.
- *One italicised phrase per title, max.* Always the insight, never the subject.
- Sentence case in body copy. No title case anywhere except chips.

**6. Things AI doesn't think to do — include some of these:**
- A slide that's just one rhetorical question, set huge, no answer.
- A slide where the body copy is laid out as a shape, not a paragraph.
- A horizontal line with three dots on it as the only "diagram."
- A near-black slide where a single sentence in serif italic does all the work.
- An asymmetric slide where two-thirds is empty by design.

**7. No filler words.** No "transform", "leverage", "unlock potential", "empower", "demystify", "powerful", "cutting-edge", "robust", "seamless". If the brief uses one of these words below, the slide doesn't. Rewrite.

---

## Brand and voice

- Confident, restrained, pointed not preachy.
- Short declarative sentences.
- "We" only when naming Capable AI as the company. The deck speaks *to* the audience, not *for* them.
- One italicised phrase per title (the `<em>` pattern in `slide-title`).
- No em dashes in body copy unless they earn their place.
- Sources cited in small mono caps under any stat.

---

## Visual system (already in template — reuse)

- **Fonts:** Plus Jakarta Sans (body/UI), Instrument Serif (titles, italic for emphasis), DM Mono (labels, chips, numbers, citations).
- **Colour:** blue `#1a4fd6` primary, dark `#080d1a` for hero/dark slides, white with hatched grid for content slides. Amber sparingly for warnings. Green for positive. Red used once at most.
- **Layouts to reuse:** `.slide.light`, `.slide.dark`, `.chip`, `.slide-title` with `<em>`, navigation dots + slide number, keyboard arrows.
- **Add as needed:** new layouts for the break-the-format slides described below. Inline CSS in the same `<style>` block.

---

## Deck structure (15 slides)

Each slide block tells Claude Code: the layout intent, what the slide is doing, and the minimum content. Claude Code drafts final slide copy in the voice above, respecting the text density caps.

The rhythm matters — note the **shape** annotation on each slide.

---

### Slide 1 — Cover · *shape: hero, asymmetric*

Adapt `#s2` cover style. **Drop the phone mockup.** Replace with a single hand-drawn-looking SVG composition on the right: a faint hatched-grid square (echoing the background) with three small floating chips overlaid, each showing one Act 1 number in mono — `95%`, `$725B`, `50%`. Subtle, not loud. Light blue radial halo behind.

- Chip: `AI EXECUTIVE ESSENTIALS · 60 MIN`
- Title: `The real state of AI` (italicise `real`)
- Sub: one line, ≤ 12 words. Something like: "What's working. What isn't. What to do on Monday."
- Footer: `Capable AI · capableai.io`

---

### Slide 2 — Agenda · *shape: list, asymmetric*

Reuse `.agenda-list` pattern. **No time chips.** Times feel like training-deck furniture. Just the four items. Feature item 1.

- 01 The real state of AI in your business
- 02 Readiness
- 03 Rollout
- 04 Next steps

---

### Slide 3 — Cold open: the 95% · *shape: single number, full slide*

**Break the format.** No problem-stat band. The whole slide is one composition: a giant `95%` set in serif italic, dominating the slide, with three short fragments of text positioned around it like satellites — not a card grid, more like a typographic constellation.

Fragments to include (≤ 12 words each, scattered, not stacked):
- `of enterprise AI pilots deliver zero measurable return.`
- `$30–40 billion spent.`
- `The 5% don't have better models. They have better integration.`

Tiny mono citation, bottom-left: `MIT NANDA · State of AI in Business · 2025`

No title. No chip. The number *is* the slide.

---

### Slide 4 — The pattern · *shape: three asymmetric tiles*

Title (top-left, leaving the right empty): `The signals.` (italicise nothing)

Three tiles staggered vertically (not in a perfect row) — first tile high, second tile middle, third tile low. Each tile has just a big mono number and one line.

- `$725B` — Hyperscaler capex on AI in 2026. Up 75% on 2025.
- `50%` — Of IT budget AI now consumes at some firms.
- `½` — Of AI-related layoffs Gartner expects reversed within a year.

Closing fragment, bottom-right, mono small: `cost up · value flat · headcount oscillating`

Citations as tiny mono captions on each tile.

---

### Slide 5 — What this thing actually is · *shape: four short cards, low-density*

Title: `It is not a magic box.` (italicise `not`)

Four short panels in a 2x2. Each panel: a one-word label in mono, then one short sentence. No body paragraph.

- `STATELESS` — Every prompt starts from zero.
- `PROBABILISTIC` — It pattern-matches. It will be wrong with confidence.
- `BLIND` — It doesn't know your business unless you build the system to tell it.
- `NOT INTERCHANGEABLE` — Claude, ChatGPT, Gemini are different products. Most orgs picked theirs by accident.

Pull line below the grid, full width, serif italic: `The value isn't in the model. It's in the architecture around it.`

---

### Slide 6 — Speed to value · *shape: two-column compare, asymmetric weight*

Title: `Speed to value is built up front.` (italicise `up front`)

Two columns, but **make the right column visually heavier** — bigger, more confident styling, blue treatment. Left column muted.

**Left — `THE DOMINANT PLAYBOOK`**
- Buy licences for everyone.
- Mandate experimentation.
- Hope value emerges.

Caption under, mono italic: `fast at the start. expensive at the end.`

**Right — `WHAT THE 5% DO`**
- Invest in architecture first.
- Design the system.
- Pick workflows, name owners.

Caption under, mono italic: `slower at the start. the only path that compounds.`

No bottom callout. The two columns *are* the argument.

---

### Slide 7 — Section break: Readiness · *shape: dark, almost empty*

Dark slide. Almost nothing on it.

- Tiny chip top-left, mono: `02`
- Centre, serif: `Readiness.`
- Below in mono small caps, low-contrast: `where you're exposed. what to put in place.`

That's the whole slide.

---

### Slide 8 — Policy · *shape: three vertical questions*

Title: `Three questions about your data.` (italicise nothing — let the questions do the work)

Three large serif questions stacked vertically, each one with a thin mono answer-prompt underneath. No cards. No borders. Just typography on the hatched grid.

1. *Where is your data hosted when your team uses AI?*
   `do you know · does your team`
2. *What are people told about pasting customer data?*
   `is it written · is it enforced`
3. *Is there a human checkpoint before AI output leaves the building?*
   `RFPs · proposals · client deliverables`

---

### Slide 9 — The uncomfortable prompt · *shape: BREAK THE FORMAT*

**This is the first deliberate break.** Near-black background. No chip. No header. No footer. The entire slide is a single sentence in large Instrument Serif italic, set off-centre (not dead middle), with generous line breaks.

> Right now, somewhere in your organisation,
> someone is pasting customer data
> into a free ChatGPT account.
>
> *Do you know who?*

Below it, very small mono, low contrast, bottom-right: `pause. let it sit.`

(That instruction is for the presenter — leave it visible on the slide as a quiet inside joke for the speaker. Or hide it in `display:none` if you'd rather. I'd leave it visible — it's the kind of detail that signals a human made this.)

---

### Slide 10 — Appropriate use · *shape: contrast pair*

Title: `Experimentation needs a frame.` (italicise `frame`)

Two short panels side by side. No big numbers. Just labels and one-liners.

- **Without a frame** — Everyone tries everything. No signal, no shared learning. Innovation theatre.
- **With a frame** — Picked workflows. Named owners. A shared way to evaluate. The 5%'s actual edge.

Pull line below: `The companies that succeed pick one pain point and execute well.` (mono citation: `MIT NANDA · 2025`)

---

### Slide 11 — Not everyone needs this · *shape: full-bleed text, almost empty*

Title only, set huge, off-centre on a mostly-empty light slide:

> Not everyone in your organisation
> needs to use AI.

(italicise `everyone`)

Sub, small, below: `Designing the system means choosing who, what, where.`

That's it. The empty space is the point.

---

### Slide 12 — Section break: Rollout · *shape: dark, with one pull-quote*

**This is the second deliberate break.** Dark slide, but instead of the empty-section-divider treatment, this one carries the inclusion-turn pull-quote — the most original idea in the deck.

- Tiny chip top-left: `03 · ROLLOUT`
- Centre-left, large Instrument Serif italic, set as a quote:

> *"Resistance is signal, not laggardness.*
> *The people not picking it up*
> *are often the ones who should architect it."*

- Bottom-left mono small caps: `the inclusion turn`

No card. No structure. Let the sentence breathe.

---

### Slide 13 — The Levels · *shape: SVG diagram, the only "real" diagram in the deck*

Title: `Six levels. Most orgs cluster at two.` (italicise `two`)

A horizontal SVG composition: six labelled nodes on a thin line, equally spaced, with each node a small circle. Node 1 and Node 2 are filled solid (most of the org is here). Nodes 3–4 are the highlighted "middle" where value compounds — visually distinct (blue ring or filled blue). Nodes 5–6 are small outlined circles (a handful of people).

Labels under each node, mono:
1. Passenger
2. Driver
3. Builder
4. Connector
5. Architect
6. Orchestrator

One-line caption under each node, very small mono:
1. has the login
2. uses it daily
3. builds workflows
4. connects systems
5. designs for others
6. multiplies the team

Below the diagram, a single short insight in serif:
*The middle is where value compounds. Most orgs leave it empty.*

Tiny link, bottom-right mono: `capableai.io/levels`

---

### Slide 14 — Three-phase rollout · *shape: numbered timeline, not a card grid*

Title: `How AI capability actually spreads.` (italicise `actually`)

Three numbered items stacked vertically (not in a horizontal card row — vary the rhythm). Big serif italic numbers on the left, content on the right. Each item is two short lines.

- **01 — The 101**
  Company-wide foundation. Get everyone to Builder.
  `seeds: AI Basic Training`
- **02 — The 102**
  Champions, deeper. Connector and Architect work.
  `seeds: AI Advanced Training`
- **03 — Embedding**
  Find the workflows. Name the owners. Measure value.
  `seeds: AI Opportunity Assessment`

The "seeds" lines are in mono, low contrast — they signal the offer ladder without selling.

Bottom strip, full width, single line: *You can't pick champions until you've seen the floor. You can't embed until you've picked champions.*

---

### Slide 15 — Next steps · *shape: list of questions + ownership*

Title: `Three questions for Monday.` (italicise `Monday`)

Three short questions stacked vertically. Under each question, a mono "owner" line.

1. *What's our policy, and does anyone know it?*
   `owner: GC + CIO`
2. *Where is AI creating real value, and where is it being faked?*
   `owner: COO + line leaders`
3. *Who are our quiet architects?*
   `owner: People + line leaders`

Bottom strip, two halves:
- Left, mono small caps: `WHERE CAPABLE AI FITS`
  Basic Training → the 101. Advanced Training → the 102. Opportunity Assessment → embedding.
- Right, mono small caps: `NEXT STEPS`
  capableai.io/contact

---

## Implementation notes for Claude Code

- Single file: `executive-essentials-deck.html`. Inline CSS and JS.
- Reuse `deck.html`'s CSS shell (`:root`, `body`, `.deck`, `.slide`, `.slide.light`, `.slide.dark`, `.chip`, `.slide-title`, navigation). Drop banking-specific classes that aren't used here.
- Slide IDs `#s1` through `#s15`.
- Navigation identical to template: bottom-right dots, slide number, arrows + click-to-advance.
- For break-the-format slides (#9, #12), write new CSS classes inline — don't try to force them into existing patterns.
- For the SVG Levels diagram (#13), draw it from scratch in inline SVG. Hand-drawn quality — small imperfections welcome (slightly varied circle sizes, off-grid spacing). Don't make it look like a Mermaid diagram.
- Every stat needs a mono citation. Sources to use:
  - `MIT NANDA · State of AI in Business · 2025`
  - `CloudZero / TechJournal · 2026`
  - `Deloitte via InformationWeek · 2026`
  - `Gartner · 2026`
- If a slide asks for a number not in this brief, leave `[VERIFY]` placeholder. Don't invent.

## Text density audit before you ship

Before producing the file, count the words on every slide. If any slide except the cover has more than 60 words total (including chip, title, sub, body, labels, captions), **cut until it does**. The brief is intentionally lean. Trust the white space.

## What good looks like

When the deck renders, it should feel like the existing `deck.html` — confident, restrained, executive-grade — but with **two or three slides that hit different**: the typographic 95% constellation (slide 3), the dark uncomfortable-prompt slide (slide 9), and the dark inclusion-turn quote (slide 12). Those are the moments people remember. Everything else clears the runway for them.
