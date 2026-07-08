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

Download and apply these skills:

1. **Anthropic Frontend Design** — This official skill prevents Claude from relying on overused fonts (like Inter or Roboto) and basic SaaS card grids. It forces the model to commit to an explicit aesthetic direction (e.g., brutalist, editorial, retro-futuristic) up front and enforces functional layering and strong typography scales.
   What to do: Install the Anthropic Frontend Design skill to define coherent design languages rather than generic outputs.

2. **UI/UX Pro Max** — This community skill gives Claude a vast database of layout styles, palettes, and design stacks. It acts as a design partner that understands how to guide user attention and build highly immersive, niche-specific frontends.
   What to do: Search community skills in your agent's ecosystem to grab the UI/UX Pro Max tool.

3. **Vercel Web Design Guidelines & Linter** — Ensures interface code matches modern web standards by auditing it against over 100 interaction and visual design rules. It automatically intercepts common design mistakes — terrible color contrast, poor touch targets, broken responsive breakpoints.
   What to do: Add the Vercel Web Design Guidelines to apply obsessive detail to every pixel on the screen.

4. **Playwright CLI (Webapp Testing)** — Lets Claude use browser automation to test form submissions, immediate UI feedback (within 100ms), and navigation. Lets the agent load the newly designed web application across multiple Chrome instances to verify how it interacts in the real world.

5. **Bencium Controlled UX Designer** — Uses a questionnaire-based approach to nail down the user experience before a single line of code is written. Prompts about flow structure (e.g., three-step checkout), visual identity, and interaction decisions, mapping out the architecture ahead of time.
