# CLAUDE.md — Kokerboom Studio project

Drop this file in the root of every client site repo. Fill in the Client brand block per project. Keep it short — this file loads into context on every session, so every line should earn its place.

## Client brand block

_Fill in per project._

- Business name:
- What the business does:
- Audience:
- Tone (Afrikaans / English / mix):
- Brand colors:
- Logo / photos:
- Any existing brand guidelines:

## Who I am

Kokerboom Studio — a one-person web design + digital consulting practice building sites for small businesses in Windhoek, Namibia. I value distinctive, on-brand work that never looks template-generated. Afrikaans and English are both fine; match the client's audience.

## Stack & workflow

- Output: multi-page static HTML/CSS. One page per file (`index.html`, `about.html`, `contact.html`, etc.). Keep it simple and dependency-light.
- Styling: hand-written CSS or Tailwind via CDN. Do not introduce build tools, bundlers, or frameworks unless I ask.
- Deploy: GitHub → Netlify. Assume a Netlify deploy preview is how I'll view results.
- Environment: I often work from an iPad, so prefer changes I can review by opening a page or a deploy preview. Don't assume a local headless browser is available unless I say so.

## Before you build — always plan first

1. Ask any question you need to pin down the brief: what the business does, its one audience, and the single job of each page. State your assumptions if I don't answer.
2. Draft a compact design plan (palette, type, layout, signature element — see below) and show it to me before writing code.
3. Layer the build: structure → content → styling. Don't dump everything in one pass.
4. After building a page, describe how to review it and what to check. If I paste a screenshot back, compare it against the plan and fix what's off.

## Design rules (non-negotiable)

- No generic AI defaults. Avoid the tells: cream background + high-contrast serif + terracotta accent (esp. near #D97757); near-black + single acid-green/vermilion accent; broadsheet hairline-rule columns. These are defaults, not choices.
- No overused fonts unless the brief demands one: skip Inter, Roboto, Arial, Space Grotesk. Pick a characterful display face + a complementary body face, chosen for this client.
- The hero is a thesis. Open with the most characteristic thing in the client's world — not a big number + label + gradient (that's the template answer).
- Structure must mean something. Only use numbered markers (01/02/03), eyebrows, or dividers when the content is actually a sequence or the label encodes real information.
- Spend boldness in one place. One signature element is the memorable thing; keep everything around it quiet. Before finishing, remove one accessory.
- Motion is deliberate. A little, where it serves the subject. Scattered effects read as AI-generated.
- Quality floor, always: responsive down to mobile, visible keyboard focus, reduced motion respected, real alt text.

## Copy rules

- Write from the user's side of the screen. Plain verbs, sentence case, no filler.
- Buttons say exactly what happens ("Send message", not "Submit") and keep the same name through the flow.
- Errors explain what went wrong and how to fix it. Empty states invite an action.
- Being specific beats being clever.

## Skills

Installed in `.claude/skills/` (from anthropics/skills):

1. **frontend-design** ✅ installed — Forces commitment to an explicit aesthetic direction (e.g., brutalist, editorial, retro-futuristic) up front instead of overused fonts and generic SaaS layouts; enforces functional layering and strong typography scales.

2. **webapp-testing** ✅ installed — Playwright-based browser automation to test form submissions, immediate UI feedback, and navigation across a running page or deploy preview.

Not yet installed — no official/public source found for these; need a repo URL or marketplace link to add them:

3. **UI/UX Pro Max** — community skill for layout styles, palettes, and design stacks.
4. **Vercel Web Design Guidelines & Linter** — audits interface code against interaction/visual design rules (contrast, touch targets, breakpoints).
5. **Bencium Controlled UX Designer** — questionnaire-based UX discovery before building.
