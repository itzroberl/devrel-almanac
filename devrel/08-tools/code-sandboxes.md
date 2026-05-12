# Code Sandboxes

Browser-based code execution environments are now an essential part of the developer-onboarding stack. Embedding a runnable example in docs reduces TTFHW from "install everything" to "type and click run."

---

## StackBlitz

- **Founded.** 2017.
- **Strengths.** WebContainers technology runs entire Node.js / npm environments in the browser via WebAssembly; near-instant boot.
- **Bolt.** StackBlitz's AI-app-building product launched in 2024 transforms text prompts into working web apps; one of the breakout AI-developer products of 2024.
- **Used by.** Angular team (official Angular docs sandboxes), many Vue/React/Svelte docs sites, MDN.

---

## CodeSandbox

- **Founded.** 2017 by Ives van Hoorne.
- **Acquired.** By Together (formerly CodeSandbox, then merged with Together AI in 2024).
- **Strengths.** Cloud development environments running real VMs; supports any language; collaborative coding.
- **API.** APIs for spinning up isolated environments programmatically — used by some DevRel teams for "click to try" experiences.

---

## Replit

- **Founded.** 2016 by Amjad Masad.
- **Positioning.** "App and site builder in your browser" with deep AI integration (Replit AI Agent, Replit Bounties).
- **Strengths.** Hundreds of integrations; mobile and web project sharing; very accessible for beginners.
- **Used by.** Education-heavy contexts; bootcamps; individual builders.

---

## CodePen

- **Founded.** 2012 by Chris Coyier, Tim Sabat, Alex Vazquez.
- **Strengths.** Front-end only (HTML/CSS/JS); social discovery; vibrant front-end community.
- **Used by.** Front-end tutorials, CSS demos, generative-art experiments.

---

## Glitch

- **Founded.** 2017 (by Fog Creek / Anil Dash team).
- **Acquired.** Multiple ownership changes; reduced investment.
- **Strengths.** Remixing model; instant Node.js apps with public URLs; favoured by web educators and prototypers.
- **Status.** Less active than during 2017–2020 peak.

---

## JSFiddle, JSBin

- **Older browser-based front-end playgrounds.** Still occasionally used; largely superseded by CodePen for new content.

---

## Specialised sandboxes

- **WebContainers** — StackBlitz's underlying technology, also licensable for embedding.
- **Sandpack** — CodeSandbox's open-source embedding library; widely used in technical blogs and docs.
- **MDX-embedded code samples** — Many docs sites embed live code samples directly via React-based components.
- **Jupyter-style notebooks** — For ML/data products, Google Colab, Kaggle Kernels, Databricks notebooks, Hex serve as the equivalent of code sandboxes.
- **Streamlit, Gradio, Hugging Face Spaces** — AI/ML demo-app platforms; effectively code sandboxes optimised for showing AI models in action.

---

## Why this matters

A working code sample reduces TTFHW dramatically. The order-of-magnitude difference between "install Node, clone the repo, run npm install, configure your API key, run the example" and "click here, type, run" determines whether many developers ever evaluate a product. Stripe's docs, Algolia's docs, and most modern API documentation embed runnable examples specifically because of this.

DevRel teams should treat sandbox embedding as table stakes for any product onboarding flow.

## See also

- [`./documentation-tools.md`](documentation-tools.md)
- [`../10-tactics/documentation-as-product.md`](../10-tactics/documentation-as-product.md)
- [`../10-tactics/sample-apps-and-demos.md`](../10-tactics/sample-apps-and-demos.md)
- [`../04-metrics/activation-metrics.md`](../04-metrics/activation-metrics.md)