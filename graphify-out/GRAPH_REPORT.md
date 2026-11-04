# Graph Report - fluent-route  (2026-11-04)

## Corpus Check
- Corpus is ~8,699 words - fits in a single context window. You may not need a graph.

## Summary
- 66 nodes · 97 edges · 6 communities
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Practice: Speak, Dictation, Ear
- Flashcards
- Placement Test Scoring
- Landing Page
- Logo, SEO And Fonts
- Stages And Progress

## God Nodes (most connected - your core abstractions)
1. `renderTest()` - 13 edges
2. `renderSpeak()` - 10 edges
3. `renderAll()` - 9 edges
4. `say() accent-aware speech` - 7 edges
5. `Accent choice accentPick() in Practice, test and tips (not in header)` - 6 edges
6. `renderShell() header + nav` - 6 edges
7. `renderToday()` - 6 edges
8. `Dictation practice (dictPool, dCheck)` - 5 edges
9. `renderMore() library + tips` - 5 edges
10. `Fluent Route site` - 5 edges

## Surprising Connections (you probably didn't know these)
- `renderShell() header + nav` --shares_data_with--> `Accent choice accentPick() in Practice, test and tips (not in header)`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 1_
- `renderTest()` --calls--> `Accent choice accentPick() in Practice, test and tips (not in header)`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 2_
- `renderHome() landing page` --calls--> `say() accent-aware speech`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 3_
- `Fluent Route site` --references--> `renderAll()`  [EXTRACTED]
  index.html → index.html  _Bridges community 1 → community 4_
- `renderAll()` --calls--> `renderTest()`  [EXTRACTED]
  index.html → index.html  _Bridges community 1 → community 2_

## Import Cycles
- None detected.

## Communities (6 total, 0 thin omitted)

### Community 0 - "Practice: Speak, Dictation, Ear"
Cohesion: 0.18
Nodes (15): Accent choice accentPick() in Practice, test and tips (not in header), Dictation practice (dictPool, dCheck), Ear training minimal pairs (EAR, newEar), High-variability phonetic training, listen() speech recognition, matchWords() LCS word match, micMsg() mic errors, PROMPTS free-talk topics (+7 more)

### Community 1 - "Flashcards"
Cohesion: 0.17
Nodes (16): CARDS flashcard deck, currentStage(), Desktop sidebar layout (.side, .today-grid) + phone bottom bar, dueCards(), grade() Leitner scheduler, Arabic/English switch (S.lang, L(), tx()), Leitner spaced repetition, NEW_PER_DAY = 10 new flashcards a day (+8 more)

### Community 2 - "Placement Test Scoring"
Cohesion: 0.17
Nodes (14): CANDO level descriptors, Computer adaptive testing, eap() ability estimate, finishTest(), LISTEN listening item bank, overall() weighted level + confidence, pCorrect() item response model, pickItem() adaptive selection (+6 more)

### Community 3 - "Landing Page"
Cohesion: 0.25
Nodes (8): Design direction: colour chapters (tasteskill), curView() / hasProgress(): new visitors land on #home, DRAW map + onlyIf(): only the visible screen renders, Landing: hero + swatch nav, input/output, four fields, seven stops, action tile, big mark footer, lpFrag() live dictation card, img/hero.jpg, clouds.jpg, jetty.jpg (Unsplash via picsum), renderHome() landing page, route() hash router

### Community 4 - "Logo, SEO And Fonts"
Cohesion: 0.29
Nodes (7): Published artifact claude.ai/artifact/67Qn5XzDPdmhtZhCMaVHUF, Fluent Route site, Fonts: Baloo Bhaijaan 2 + Readex Pro, Logo: route ending in speech bubble (LOGO, logo.svg), Animations (rise, stagger, flip, pulse, pop), SEO head: meta, Open Graph, JSON-LD, canonical, robots.txt, sitemap.xml, site.webmanifest, og.png, icons

### Community 5 - "Stages And Progress"
Cohesion: 0.50
Nodes (4): CEFR levels, LV levels A1-Native, STAGES with checklists, UOE grammar and reading item bank

## Knowledge Gaps
- **20 isolated node(s):** `micMsg() mic errors`, `PROMPTS free-talk topics`, `High-variability phonetic training`, `Shadowing`, `USUK word table` (+15 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 22 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `renderTest()` connect `Placement Test Scoring` to `Practice: Speak, Dictation, Ear`, `Flashcards`, `Landing Page`, `Stages And Progress`?**
  _High betweenness centrality (0.441) - this node is a cross-community bridge._
- **What connects `micMsg() mic errors`, `PROMPTS free-talk topics`, `High-variability phonetic training` to the rest of the system?**
  _20 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Why does `renderAll()` connect `Flashcards` to `Practice: Speak, Dictation, Ear`, `Placement Test Scoring`, `Landing Page`, `Logo, SEO And Fonts`?**
  _High betweenness centrality (0.372) - this node is a cross-community bridge._
- **Why does `renderSpeak()` connect `Practice: Speak, Dictation, Ear` to `Flashcards`?**
  _High betweenness centrality (0.182) - this node is a cross-community bridge._