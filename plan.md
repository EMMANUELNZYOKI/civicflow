# CivicFlow implementation plan

## Product
CivicFlow is a responsive community service navigator. It solves the problem of residents struggling to find trustworthy local support by organizing services into clear categories, comparison details, and a guided request form.

## Design
Three directions considered:
- Civic Signal: confident public-service aesthetic with deep civic blue, warm amber accents, crisp information panels, and editorial typography. Probability 0.04.
- Garden Commons: human-centered community look with leafy green, terracotta warmth, and friendly type. Probability 0.03.
- Night Transit: high-contrast wayfinding interface with navy, electric mint, and modular blocks. Probability 0.02.

Chosen direction: **Civic Signal**.

- Design movement: editorial civic-tech wayfinding.
- Core principles: trustworthy hierarchy, fast scanning, inclusive language, and visible progress.
- Color philosophy: deep navy establishes reliability; amber marks action and warmth; pale blue-gray surfaces keep information calm and readable.
- Layout paradigm: offset editorial panels and a left-edge service rail rather than a generic centered card grid.
- Signature elements: amber route markers, oversized numeric section labels, and dotted “service path” dividers.
- Interaction philosophy: controls give immediate status feedback and never hide the next step.
- Animation: short fade/slide reveals, gentle hover lift, and a reduced-motion fallback.
- Typography: Public Sans system fallback with bold display headings and compact uppercase labels.
- Brand essence: “Find the right help, without the runaround.” Personality: practical, reassuring, neighborly.
- Voice: direct and human. Example CTAs: “Find a service” and “Send a support request.”
- Wordmark: CIVICFLOW with a two-line route marker icon.
- Signature color: Civic Navy #123B5D.

## Structure
- `index.html`: landing page and impact counters.
- `about.html`: problem, client/server explanation, hosting and trends.
- `services.html`: searchable/filterable service directory and comparison table.
- `gallery.html`: image-led community story plus audio and video media.
- `contact.html`: validated support request form and contact channels.
- `styles.css`: shared responsive visual system.
- `script.js`: navigation toggle, counters, service filtering, accordions, form validation, and feedback.
- `public/manus-routes.json`: complete route manifest.

## Technical approach
Static HTML/CSS/JavaScript keeps the submission easy to inspect and demonstrates core Internet Programming concepts directly. JavaScript uses DOM methods, arrays, event listeners, conditionals, loops, and form validation. The site is designed to be deployable on shared hosting, an application server, or a dedicated server.
