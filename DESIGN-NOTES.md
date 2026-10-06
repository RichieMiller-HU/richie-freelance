# Design notes, v2 (2026-10-06)

## References (what makes them feel premium)

1. **Joshua Baker, joshuabaker.com** (a1.gallery, "dark typographic AI portfolio"). One long first-person sentence as the hero, set huge; everything else is quiet. Credibility comes from the sentence, not from tiles. Restraint: black, white, one typeface scale, no decoration.
2. **Maximilian Kaspar, maximiliankaspar.com** (a1.gallery, Swiss designer). Strict grid, lower-case editorial statement, each project gets a full-width row with generous whitespace above and below; a single "scroll down" cue; hierarchy made by scale only.
3. **Sarah Drasner / Yuto Takahashi** (socialanimal.dev "best designed 2026"): reading typography with generous line height, minimal text next to very large imagery, page feels like paging through a printed portfolio. Godly's 2026 selection in general leans on grid discipline, considered type scale and whitespace rather than motion gimmicks.

## Direction (5 lines)

1. Printed-matter feel: warm bone paper, near-black ink, hairline rules, one ink-dark "chapter" for Selected work; no gradients, no glows, no cards, no tiles.
2. Type carries the design: Instrument Serif (display, italic for emphasis) at 8 to 12vw, Hanken Grotesk 300/400 for reading, DM Mono for small index labels (01, 02, "Selected work").
3. Editorial grid: label column left, content right; large numbered list rows with hairlines instead of icon cards; left-aligned, asymmetric, lots of air.
4. The photo is a cut-out, black and white, placed large and bleeding off the hero, overlapped by the headline; it parallaxes slowly on scroll.
5. Motion is Lenis smooth scroll plus GSAP line reveals, a drawn SVG flow diagram and a number count-up; everything is fully visible with no JS or with prefers-reduced-motion.
