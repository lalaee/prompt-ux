# prompt:UX 2027 talk proposal

Research date: 23 October 2026. Conference: prompt:UX, 24 & 25 February 2027, AMANO East Side, Berlin.

## Before you pitch

Every page of promptux.ai currently says: "there are no more speaker slots available for 2027. Therefore, please do not apply." The program still shows two "To be announced" talks (13:00 and 13:40 on 24 Feb), but those are most likely already promised.

So don't send a cold application. Write to Luciano Lykkebo (Founder & Event Director, promptux@westwerk.events) instead:

- Ask to be considered as a backup speaker if a 2027 slot falls through.
- Ask to be considered for the next edition (they also ran Stockholm in 2025).
- Attach the one-paragraph abstract below and a link to past work, so he has something concrete.

## What they already have for 2027

| Slot | Speaker | Topic |
|---|---|---|
| Talk | Philip Illum Thonbo, Trifork | Design systems and AI |
| Talk | Rinaldo Ugrina, Baymard | Strategic storytelling |
| Talk | Henrik Harsbo, PensionDanmark | AI for real life: users who don't want a chat |
| Talk | Christian Kuhn, Optimizer | "Don't make me prompt!": interfaces users like |
| Mini workshop | Niek van Esch, Centraal Beheer | Design with flow (pen and paper) |
| Workshop | Christian Kuhn | Microsoft's HAX principles for human-AI experiences |
| Workshop | Thomas Van den Bossche, Odisee | Vibe coding for UX designers |

Already covered, so avoid: vibe coding and prototyping, design systems with AI, chat vs. non-chat end-user UI, and trust/ethics principles.

Missing from the lineup: how designers work *with agents* day to day, what makes AI output look good or bad (taste), and designing for agents as users.

The site's own framing is "AI skills for 2027", "advanced AI UX topics, concrete problems and use cases", and "prepare your AI strategy for the next year". Past speakers come from big product companies (Google, Microsoft, Booking, Zalando, IKEA) and specialist practitioners.

## What the data says

**Google Trends, worldwide, past 12 months** (checked 23 Oct 2026; reproduce with [Claude Code vs MCP server](https://trends.google.com/trends/explore?date=today%2012-m&q=Claude%20Code,MCP%20server) and [prompt engineering vs AI agent](https://trends.google.com/trends/explore?date=today%2012-m&q=prompt%20engineering,AI%20agent))

- "prompt engineering" has collapsed. It peaked at 18 in Feb 2026 and is now 2 (on a scale where "AI agent" peaked at 100). A talk *about prompting* is now a dated pitch, even at a conference called prompt:UX.
- "Claude Code" is by far the biggest term in the tool space. It peaked in late March 2026 and is still about 34.
- "Claude Design" jumped in April 2026 and has held steady. Its rising related queries are all about *skills*: "frontend design skill claude", "claude code frontend design skill", "claude web design skill".
- "Claude skills" is rising again (7 → 10 over the last two months), while general terms like "AI design" and "AI agent" are falling.
- Breakout queries: "context engineering skill claude", "agent skills for context engineering", "stop slop skill", and "your ai slop bores me".
- "generative UI" is still tiny, but its breakouts are protocol names: A2UI, AG-UI, MCP Apps. It's early but heading somewhere.

**YouTube (videos from 2026)**

- "How to Use Claude Skills as a Designer" (Griffin Wooldridge): 321K views
- "Insane Claude Design Skills You Need To Actually Build Beautiful Sites" (AI LABS), about steering Claude away from its default look: 355K views in one month
- "How to Use Claude Design Better Than 99% of People" (Jack Roberts): 56K views in 13 days
- "7 INSANE Claude Design Use Cases": 39K views

**Industry reports**

- [Lyssna, UX design trends 2026](https://www.lyssna.com/blog/ux-design-trends/): about 60% of designers expect agents that act for users to have a major impact this year.
- [Figma's 2026 AI report](https://www.figma.com/blog/2026-ai-report/) (24 Jun 2026): designers taking part in development rose from 21% to 41%. An earlier note here said "51% of designers building AI products work on agents"; that figure could not be found in Figma's report, so don't use it.
- The open-source "Taste Skill" (instruction files to make agents avoid the template look) passed 64,000 GitHub stars.

## Topic options

### 1. Recommended: Your taste is now a file

**Working title:** *Past the prompt: teaching AI agents your design taste*

**Pitch in one line:** Prompting is over. The designers getting great output from AI in 2026 write *skills*: reusable files that hold their judgment, their system, and their "never do this" list, so every agent run starts out knowing what they know.

**Why it fits:**
- It answers the conference name head-on. The organisers will like a talk that moves "prompt" UX forward.
- It's the gap in the 2027 lineup. Thonbo covers design systems (components and tokens), Kuhn covers end users not prompting, and Van den Bossche covers prototyping. Nobody covers how a designer's *judgment* gets into the machine.
- It's where the search and video interest is now (see above).
- It's concrete. You can show a real skill file, the output before and after, and the failures that made you add each rule.

**Takeaways for the audience:**
1. Why one-off prompts produce the "AI slop" look: AI picks the most average choice when you don't give it a direction.
2. The anatomy of a design skill: principles, measured rules, banned defaults, references, and a check step.
3. How to turn a review comment you keep repeating into a rule an agent follows every time.
4. How a team shares, versions, and argues about these files like a design system.

**Abstract (about 100 words, ready to paste):**

> Searches for "prompt engineering" have fallen to almost nothing this year, but AI-made interfaces still look the same: the same gradient, the same three cards, the same safe type. The problem was never the prompt. It's that our design judgment lives in our heads and agents start every run from zero. In this talk I show how I write design skills: plain files that teach Claude, Figma's agent and others the principles, measurements and banned defaults I'd otherwise repeat in every review. Using real before-and-after work, you'll leave knowing how to capture your team's taste once and get it back in every output.

### 2. Your AI slop bores me

**Working title:** *Your AI slop bores me: taste as the last differentiator*

A provocative, opinionated version of option 1. It's less about method and more a critique of the generic look, plus a framework for spotting and removing it. It's good for a keynote-style slot and audiences love it, but it's thinner on the "skills to take home" the site promises. Use it as the title for option 1 if you want more punch.

### 3. Designing for the second user

**Working title:** *Designing for the second user: when your interface is read by an agent*

Products now serve people *and* the AI agents acting for them. This talk covers what changes: semantic structure, predictable components, agent-readable states, and the new generative-UI protocols (MCP Apps, A2UI). It's forward-looking and fits "prepare your AI strategy for next year". Search volume is still small, though, and you'd need real project examples to make it credible.

### 4. The designer's loop with agents

**Working title:** *Figma to agent and back: a designer's real working loop in 2027*

A practical walk through a real project: extracting from Figma through MCP, building with Claude Code, checking fidelity, and pushing changes back to Figma. It's highly concrete, but it sits close to the vibe-coding workshop, so you'd need to frame it as *production fidelity*, not prototyping.

## Recommendation

Lead with option 1 ("Past the prompt"), and keep "Your AI slop bores me" in your pocket as an alternative title. It's the strongest match between what's trending, what's missing from their 2027 lineup, and the conference's own name.

## Decision (23 Oct 2026)

The speaker chose **option 4, "Figma to agent and back"**, over the recommendation. See [HANDOFF.md](HANDOFF.md) for the developed version of that talk and the next steps.
