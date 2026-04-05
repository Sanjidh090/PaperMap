# PaperMap - Interactive Research Paper Library

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Static Site](https://img.shields.io/badge/Stack-HTML%2FCSS%2FJS-blue)](https://github.com/AdilShamim8/PaperMap)
[![Live Demo](https://img.shields.io/badge/Live-papermap.vercel.app-ff6b6b)](https://papermap.vercel.app/)

PaperMap turns landmark AI papers into interactive, production-quality explainers.

The goal is simple: preserve research accuracy while making complex ideas easier to understand through visual breakdowns, interactive demos, and structured teaching flow.

## Live Experience

- Home: https://papermap.vercel.app/
- Attention Is All You Need: https://papermap.vercel.app/Attention_Is_All_You_Need.html
- Language Models are Few-Shot Learners: https://papermap.vercel.app/Language_Models_are_Few_Shot_Learners.html
- Training Language Models to Follow Instructions with Human Feedback: https://papermap.vercel.app/Training_Language_Models_to_Follow_Instructions_with_Human_Feedback.html

## Key Features

- Research-accurate content grounded in original papers
- Interactive visual learning components
- Mobile-first responsive layouts
- Accessible semantics and keyboard-friendly navigation
- Pure static architecture with no build pipeline
- Consistent visual system across all explainers

## Production Readiness

This repository is structured for static production deployment:

- Canonical and social metadata in each page
- External link hardening for new-tab links
- Referrer policy metadata
- robots.txt for crawler guidance
- sitemap.xml for indexing support
- Dedicated 404.html for user-friendly missing routes

## Repository Structure

```text
PaperMap/
|-- 404.html
|-- Attention_Is_All_You_Need.html
|-- index.html
|-- Language_Models_are_Few_Shot_Learners.html
|-- Training_Language_Models_to_Follow_Instructions_with_Human_Feedback.html
|-- favicon.svg
|-- robots.txt
|-- sitemap.xml
`-- README.md
```

## Local Development

Option 1 (quick preview):

- Open index.html directly in your browser

Option 2 (recommended local server):

```bash
# Python
python -m http.server 8080

# Node.js
npx serve .
```

Then open:

- http://localhost:8080

## Deployment

PaperMap is compatible with any static host:

- Vercel
- Netlify
- GitHub Pages
- Cloudflare Pages

GitHub Pages setup:

1. Push repository to GitHub
2. Open Settings -> Pages
3. Set Source to Deploy from a branch
4. Select branch main and folder /(root)
5. Save and wait for publish

## Adding a New Paper

1. Create a new HTML file using clear Pascal_Case naming
2. Start from an existing explainer to preserve structure and style consistency
3. Add a new paper card in index.html
4. Add complete metadata in the head section
5. Verify desktop, mobile, and keyboard accessibility
6. Update sitemap.xml when adding public pages

## Recommended QA Before Release

- Validate internal navigation links
- Test responsive behavior on narrow screens
- Confirm no console errors in major browsers
- Verify social preview tags on each page
- Recheck robots.txt and sitemap.xml entries

## Attribution

PaperMap explainers are educational derivative works based on original publications.

Current papers covered:

- Attention Is All You Need (Vaswani et al., 2017)
- Language Models are Few-Shot Learners (Brown et al., 2020)
- Training Language Models to Follow Instructions with Human Feedback (Ouyang et al., 2022)

## License

Licensed under the MIT License.
