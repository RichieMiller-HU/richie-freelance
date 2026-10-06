# Design notes, v3 (2026-10-06)

## References (what makes them feel premium)

1. **Joshua Baker, joshuabaker.com** (a1.gallery, "dark typographic AI portfolio"). One long first-person sentence as the hero, set huge; everything else is quiet. Credibility comes from the sentence, not from tiles. Restraint: black, white, one typeface scale, no decoration.
2. **Maximilian Kaspar, maximiliankaspar.com** (a1.gallery, Swiss designer). Strict grid, lower-case editorial statement, each project gets a full-width row with generous whitespace above and below; a single "scroll down" cue; hierarchy made by scale only.
3. **Sarah Drasner / Yuto Takahashi** (socialanimal.dev "best designed 2026"): reading typography with generous line height, minimal text next to very large imagery, page feels like paging through a printed portfolio. Godly's 2026 selection in general leans on grid discipline, considered type scale and whitespace rather than motion gimmicks.

## Direction (5 lines)

1. Printed-matter feel: warm bone paper, near-black ink, hairline rules, one ink-dark "chapter" for Selected work; no gradients, no glows, no cards, no tiles.
2. Type carries the design: Geist 650 to 800 (self-hosted variable woff2, Latin subset, 400 to 800) with -0.035 to -0.05em tracking for headlines, Geist 400 for reading, Geist Mono for small index labels. Emphasis by colour (ink vs muted grey), never italics. v3 replaced Instrument Serif after owner feedback (too "magazine").
3. Editorial grid: label column left, content right; large numbered list rows with hairlines instead of icon cards; left-aligned, asymmetric, lots of air.
4. The photo is a cut-out, black and white, placed large at the right of the hero beside the headline (no overlap, no blend modes); light transform-only parallax on desktop.
5. Performance first (v3): no GSAP, no Lenis, no grain overlay, no mix-blend, no filters. Native scroll; IntersectionObserver adds .in for CSS opacity/transform reveals; CSS load animation on the hero; vanilla count-up. Everything visible without JS or with prefers-reduced-motion. Page weight about 87 KB uncompressed.
