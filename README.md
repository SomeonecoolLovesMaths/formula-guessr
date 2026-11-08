# Formula Guessr — JEE Recall Studio

A static, browser-based formula-recognition and active-recall website for JEE Mathematics, Physics and Chemistry.

## Formula bank

The current bank contains **987 cards**:

| Subject | Cards | Easy | Medium | Hard |
|---|---:|---:|---:|---:|
| Mathematics | 648 | 88 | 404 | 156 |
| Physics | 176 | 44 | 71 | 61 |
| Chemistry | 163 | 23 | 61 | 79 |
| **Total** | **987** | **155** | **536** | **296** |

Mathematics includes a substantial hard-level expansion in conics (parabola, ellipse, hyperbola and general conic properties) and trigonometry (multiple-angle, finite-sum, product-to-sum, Chebyshev and triangle identities). Physics now spans mechanics, fluids, thermal physics, waves, electrostatics, current electricity, magnetism, induction, AC, optics and modern physics. Chemistry spans solutions, equilibria, electrochemistry, kinetics, atomic structure, bonding, coordination chemistry, thermodynamics and organic transformations.

Every MCQ has a correct expression and three distractors. Physics choices are formatted consistently as relations/equations, so an equation is not identifiable merely because it includes a left-hand side while the alternatives do not.

## Run locally

Open `index.html` in a modern browser. The site is static; no server, account, database, build step or installation is required. An internet connection is used for Google Fonts and KaTeX mathematical typesetting. KaTeX is loaded from jsDelivr with an unpkg fallback and each formula is rendered directly into its own element (rather than relying on delimiter-scanning over generated HTML). The formula data and application code are local files.

## GitHub Pages

Upload the files in this folder to the root of a GitHub repository, enable GitHub Pages for the desired branch and folder, and open the published URL.

## Interface

- Dark and light themes, switchable from the top bar.
- Floating mathematical glyphs, an orbital hero graphic and a custom crosshair cursor with a subtle pointer-following glow on desktop.
- Responsive layout for desktop, tablet and mobile.
- Practice sessions with subject, difficulty, chapter, class and question-count filters.
- Immediate MCQ feedback, explanations and formula conditions.
- Searchable formula library and flashcards.

The theme choice is session-only; the site does not save scores, filters or personal data. The cursor effect automatically disables on touch devices and when reduced motion is requested.

## Files

- `index.html` — page shell, external typography/typesetting resources and script references.
- `styles.css` — responsive theme, floating background, cursor aura and visual design.
- `app.js` — practice sessions, consistent Physics option formatting, light/dark toggle, pointer effects, direct KaTeX rendering and interactions.
- `math-bank.js` — Mathematics formula bank.
- `extra-bank.js` — additional Mathematics, Physics and Chemistry formula banks.
- `.nojekyll` — tells GitHub Pages not to apply Jekyll processing.

## Difficulty definitions

- **Easy:** fundamental facts and immediate-recall identities.
- **Medium:** essential textbook and frequently used JEE formulas.
- **Hard:** specialised, easy-to-confuse or memory-intensive results.

## Coverage note

This is a broad, curated recall bank, not a claim of exhaustive syllabus coverage. Some advanced identities and transformations are supplementary. Verify conventions, assumptions and exam relevance against your current syllabus and preferred textbook. Formula recognition is only one part of preparation; derivations and problem-solving remain essential.
