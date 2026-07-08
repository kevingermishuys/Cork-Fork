# CLAUDE.md — Kokerboom Studio project

Drop this file in the root of every client site repo. Fill in the Client brand block per project. Keep it short — this file loads into context on every session, so every line should earn its place.

## Client brand block

- Business name: The Cork & Fork Restaurant
- What it does: Casual-contemporary restaurant in Windhoek, Namibia (Centaurus Street). Breakfast through dinner, full bar/cocktails, garden + indoor seating, kids welcome. 4.3★ on TripAdvisor, ~3,300 IG followers (@thecorkandfork).
- Hours: Tue–Sat 7am–10pm, Sun 7am–3pm, Mon closed.
- Contact: +264 81 707 2046. Website domain TBD.
- Audience: Local Windhoek regulars + tourists/hotel guests (reviews from Argentina, Sweden, India, US). Families welcome (kids' menu, play area on the lawn).
- Tone: English, playful/pun-heavy ("What the fork is for dinner?", "Time to uncork and unwind", "May the fork be with you", "Tonight's forecast: 99% chance of wine") layered over a genuinely upscale-casual menu.
- Menu highlights: Namibian Kapana beef strips, oryx game loin, butcher's block steaks (fillet/rump/T-bone/rib eye), malva pudding, crème brûlée trio — local specialties alongside international comfort food (pizza, pasta, burgers, tacos/quesadillas). Full bar with signature cocktails. Platters to share, full kids' menu.
- Brand colors: mustard/gold (`cork`) + maroon/burgundy (`fork`) from the wordmark, sage-green textured wallpaper indoors, warm dark wood furniture, brick-paved garden patio.
- Logo: hand-drawn line-art wine bottle pouring into a fork, forming a cursive "The"; "cork" (mustard) + "fork" (maroon) below, "restaurant" subtitle in grey.
- Signature ambiance: stretch-tent shaded garden patio, large lawn with gazebos and a kids' play area, indoor dining room with punny framed poster art on sage wallpaper, glass-walled corridor bar with string lighting opening onto the garden.
- Assets on hand: logo, full menu (all categories, priced in N$), a handful of decent original photos (garden lawn, two interior/patio shots, one Instagram wine-pairing graphic), plus lower-res TripAdvisor review photos. Treat as preview-quality — crop to fit; swap for real photography later.
- Site goal: equal weight on visual storytelling (photos/menu/ambiance) and driving a visit — phone number and location/hours should be persistently visible as the de facto "booking" CTA (no online reservation system).
- Menu display: full menu on-page (not a PDF link), organized by category.

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

Installed in `.claude/skills/`:

1. **frontend-design** ✅ (anthropics/skills) — Forces commitment to an explicit aesthetic direction (e.g., brutalist, editorial, retro-futuristic) up front instead of overused fonts and generic SaaS layouts; enforces functional layering and strong typography scales.
2. **webapp-testing** ✅ (anthropics/skills) — Playwright-based browser automation to test form submissions, immediate UI feedback, and navigation across a running page or deploy preview.
3. **responsive-design** ✅ (lotfb86/web-design-skills) — Mobile-first breakpoints, fluid typography, container queries, responsive images. Framework-agnostic, applies directly to hand-written CSS.
4. **web-design-guidelines** ✅ (lotfb86/web-design-skills, Vercel's Web Interface Guidelines) — Reviews finished UI code against ~100 interaction/accessibility rules (contrast, touch targets, focus states, breakpoints).

Deliberately skipped from lotfb86/web-design-skills: `theme-factory`, `website-rebuild`, `local-business-rebuild`, `azerbaijan-website-build`. Those assume an Astro + Tailwind v4 + Vercel pipeline, which conflicts with the stack rules above (static HTML/CSS, no build tools, deploy to Netlify). Revisit only if a project explicitly calls for that stack.

Not yet installed — no working source found:

5. **UI/UX Pro Max** — need a repo/marketplace link.
6. **Bencium Controlled UX Designer** — need a repo/marketplace link.
7. **Astro website skill (Leon Furze)** — blog post is bot-blocked; need the direct GitHub URL. Also likely the same Astro/Tailwind/Vercel conflict as above.
