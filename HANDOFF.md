# Agent handoff: prompt:UX 2027 talk

Last updated: 23 October 2026. Read this first, then `talk-proposal.md`.

## Goal

The user (Olalekan Isaac, a product/UX designer) wants to speak at **prompt:UX 2027**, an AI-for-UX conference on 24–25 February 2027 at the AMANO East Side hotel in Berlin. Site: https://www.promptux.ai/. This repo holds the talk proposal and its supporting material.

## Status

| Step | State |
|---|---|
| Read the conference site, program, workshops, alumni speakers | Done |
| Trend research (Google Trends, YouTube, web) | Done, see `talk-proposal.md` |
| Shortlist four topic options | Done, see `talk-proposal.md` |
| User picks a topic | Done: **"Figma to agent and back"** (option 4) |
| Full abstract and talk outline for the chosen topic | **Not started** |
| Email to the event director | **Not drafted, not sent** |
| Slides | Done: 16 slides in Figma with the ZEOS One case, see below |
| Bio, demo | Not started |

## Blocker: the speaker slots are closed

Every page of promptux.ai says: "there are no more speaker slots available for 2027. Therefore, please do not apply." The program shows two "To be announced" talks (24 Feb, 13:00 and 13:40), probably already promised.

So **don't** submit through a form. The plan is a personal email to **Luciano Lykkebo**, Founder & Event Director, promptux@westwerk.events, asking to be:
1. a backup speaker if a 2027 slot falls through, or
2. considered for the next edition (they also ran Stockholm in 2025).

Never send email for the user. Draft it and let them send it.

## The chosen talk: "Figma to agent and back"

**Working title:** *Figma to agent and back: a designer's real working loop in 2027*

**Core idea:** AI agents can turn a Figma frame into code in minutes, but the result drifts from the design (guessed spacing, swapped fonts, hidden layers rendered, icons redrawn by eye, made-up token values). And once the code changes, the Figma file goes stale. The talk is about **fidelity in both directions**.

**The loop the talk demonstrates on one real project:**
1. **Figma → agent:** Pass structured design data through the Figma MCP (positions, tokens, type, vectors, visibility), not screenshots. Data lets the agent measure instead of guess.
2. **Agent builds:** Build from those numbers with the design system's real components.
3. **Check, don't eyeball:** Export the frame from Figma and diff it pixel by pixel against the built screen.
4. **Agent → Figma:** Push code changes back into Figma as editable layers built from library components, so Figma stays the source of truth.
5. **Make it repeatable:** Turn every fix for drift into a rule (a skill) the agent follows next time.

**Audience takeaways:**
- When to give an agent data and when a screenshot is enough
- A fidelity check they can run on any build
- How to keep Figma the source of truth instead of an archive of old designs
- The failure modes to expect, and the rule that fixes each

**Draft one-line pitch:**
> AI can turn a Figma frame into code in minutes, but "close enough" isn't the design. This talk shows a working loop for getting from Figma to agent and back with real fidelity: structured design data in, pixel-level checks, changes pushed back to Figma, and rules that stop the same drift from happening twice.

**Positioning (important):** The 2027 program already has a full-day workshop, "Vibe Coding for UX Designers" (Thomas Van den Bossche), and a talk on "Design systems and AI" (Philip Illum Thonbo). Frame this talk as **production fidelity, not prototyping**, and as a *working loop*, not a component library. That's what makes it different.

**The user's own material:** The user already has Claude Code skills that cover this loop, which can become the demo:
- `figma-verbatim-to-code`: extracts a Figma selection through the Sunnyside Figma MCP plugin bridge, implements it exactly, and verifies pixel for pixel against a Figma export (steps 1–3)
- `figma:figma-generate-design`: pushes code back into Figma using design system components (step 4)
- `tracing-raster-art`: rebuilds icons that only exist as images as accurate vectors
- A related local project: `~/Downloads/Code/Prompt-alone-framer-fidelity-exporter`

The demo project is the ZEOS One work in `lalaee/zd` (see the slide deck section).

## Slide deck (23 Oct 2026)

Figma file: https://www.figma.com/design/rmhcA2eK2thS8TO9iYsnHn (a copy of the Zalando Wintersports LAAX file), page **"🎤 Talk: Figma to agent and back"**, section "Slides".

- 16 frames at 1920×1080: title, "Close enough isn't the design", drift, Figma goes stale, the case (ZEOS One), the loop, steps 01 to 03, "Measure, don't guess", steps 04 and 05, what doesn't work yet, takeaways, live demo, thank you.
- **Use case and demo: the user's ZEOS One work in https://github.com/lalaee/zd** (private). The drift examples, numbers (5 libraries, 2,835 variants, 110 semantic colours, 46 playground screens, 31 wireframes), commands, the validator rules and the rules table all come from that repo's `README.md`, `docs/agent-summary.md`, `design-system/zeos/` and the `zeos-screen` / `zeos-to-figma` / `copy-lint` skills.
- Screenshots on slides 05, 09 and 15 come from `zd/playground/docs/figma-next-steps/` (`1-viewer.png`, `4-figma-vs-playground.png`).
- Local components on the same page: `Slide chrome` (header/footer, Section text property) and `Card` (Number, Title, Body text properties).
- **Deck style only** comes from the Wintersports toolkit: layout, colours (black, off-black #2A2C31, orange #FF4C00), Zalando Sans (open source) and carving lines. No Zalando logo, play mark or campaign content.
- Open: ZEOS One is an internal Zalando product, so the user needs approval before showing it publicly. The website or LinkedIn link on the thank-you slide is still a placeholder.

## Supporting evidence (details in `talk-proposal.md`)

- YouTube 2026 videos on Claude Code + Figma MCP workflows for designers are common (for example "Claude Code + Figma Design System (Designer Workflow Test)" and "Design with Claude Code: The Designer's Guide").
- Google Trends (worldwide, 12 months): "Claude Code" is the dominant tool term; "MCP server" peaked in June 2026; "prompt engineering" has collapsed to about 2/100.
- Figma's 2026 AI report, as cited elsewhere: 51% of designers building AI products work on agents (up from 21%).

## Next steps for the next agent

1. Demo project chosen: ZEOS One (`lalaee/zd`). Still ask for results such as time saved per screen.
2. Write a full ~150-word abstract, a 30–40 minute talk outline (sections with timings), and a short speaker bio. Put them in `talk-proposal.md` or a new `figma-to-agent-talk.md`.
3. Draft the email to Luciano Lykkebo (backup or next-edition pitch, abstract included). Save it as `email-draft.md`. Don't send it.
4. Later: slides and a recorded demo of one screen going round the full loop.

## Writing style the user expects

Plain, direct language. Avoid AI-writing tells: em dashes in copy, "not X but Y" constructions, groups of three, and words like "delve" or "seamless".
