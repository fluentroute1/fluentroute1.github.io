# Graph Report - fluent-route  (2026-11-04)

## Corpus Check
- Corpus is ~7,367 words - fits in a single context window. You may not need a graph.

## Summary
- 57 nodes · 79 edges · 9 communities
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Library And Resources
- Practice: Speak, Dictation, Ear
- Flashcards
- Logo, SEO And Fonts
- Placement Test Scoring
- Shell, Language And Accent
- Site Core
- Site Core
- Stages And Progress

## God Nodes (most connected - your core abstractions)
1. `renderTest()` - 11 edges
2. `renderAll()` - 9 edges
3. `renderSpeak()` - 9 edges
4. `say() accent-aware speech` - 6 edges
5. `renderShell() header + nav` - 5 edges
6. `eap() ability estimate` - 5 edges
7. `finishTest()` - 5 edges
8. `Fluent Route site` - 5 edges
9. `Dictation practice (dictPool, dCheck)` - 5 edges
10. `renderMore() library + tips` - 4 edges

## Surprising Connections (you probably didn't know these)
- `renderToday()` --calls--> `dueCards()`  [EXTRACTED]
  index.html → index.html  _Bridges community 2 → community 0_
- `Fluent Route site` --references--> `renderAll()`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 3_
- `renderAll()` --calls--> `renderShell() header + nav`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 5_
- `renderAll()` --calls--> `renderSpeak()`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 1_
- `renderAll()` --calls--> `renderTest()`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 7_

## Import Cycles
- None detected.

## Communities (9 total, 0 thin omitted)

### Community 0 - "Library And Resources"
Cohesion: 0.28
Nodes (9): currentStage(), renderAll(), renderMore() library + tips, renderPath(), renderToday(), RES resource library, route() hash router, stageDone() (+1 more)

### Community 1 - "Practice: Speak, Dictation, Ear"
Cohesion: 0.31
Nodes (9): Dictation practice (dictPool, dCheck), Ear training minimal pairs (EAR, newEar), High-variability phonetic training, LISTEN listening item bank, PROMPTS free-talk topics, renderSpeak(), say() accent-aware speech, SENTS repeat-after-me sentences (+1 more)

### Community 2 - "Flashcards"
Cohesion: 0.25
Nodes (8): CARDS flashcard deck, dueCards(), grade() Leitner scheduler, Arabic/English switch (S.lang, L(), tx()), Leitner spaced repetition, place (placement result), renderWords(), store (localStorage wrapper)

### Community 3 - "Logo, SEO And Fonts"
Cohesion: 0.29
Nodes (7): Published artifact claude.ai/artifact/67Qn5XzDPdmhtZhCMaVHUF, Fluent Route site, Fonts: Baloo Bhaijaan 2 + Readex Pro, Logo: route ending in speech bubble (LOGO, logo.svg), Animations (rise, stagger, flip, pulse, pop), SEO head: meta, Open Graph, JSON-LD, canonical, robots.txt, sitemap.xml, site.webmanifest, og.png, icons

### Community 4 - "Placement Test Scoring"
Cohesion: 0.40
Nodes (6): Computer adaptive testing, eap() ability estimate, matchWords() LCS word match, pCorrect() item response model, pickItem() adaptive selection, selfCheck() scoring asserts

### Community 5 - "Shell, Language And Accent"
Cohesion: 0.40
Nodes (4): US/UK accent switch (S.accent), listen() speech recognition, micMsg() mic errors, renderShell() header + nav

### Community 6 - "Site Core"
Cohesion: 0.40
Nodes (4): finishTest(), overall() weighted level + confidence, vocabScore() Milton bands, X_Lex vocabulary size method

### Community 7 - "Site Core"
Cohesion: 0.50
Nodes (4): CANDO level descriptors, renderTest(), Test mistakes review (tst.wrong), VOCAB X_Lex word list with fake words

### Community 8 - "Stages And Progress"
Cohesion: 0.50
Nodes (4): CEFR levels, LV levels A1-Native, STAGES with checklists, UOE grammar and reading item bank

## Knowledge Gaps
- **17 isolated node(s):** `route() hash router`, `USUK word table`, `Leitner spaced repetition`, `micMsg() mic errors`, `PROMPTS free-talk topics` (+12 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 19 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `renderAll()` connect `Library And Resources` to `Practice: Speak, Dictation, Ear`, `Flashcards`, `Logo, SEO And Fonts`, `Shell, Language And Accent`, `Site Core`?**
  _High betweenness centrality (0.493) - this node is a cross-community bridge._
- **What connects `route() hash router`, `USUK word table`, `Leitner spaced repetition` to the rest of the system?**
  _17 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Why does `renderTest()` connect `Site Core` to `Library And Resources`, `Practice: Speak, Dictation, Ear`, `Flashcards`, `Placement Test Scoring`, `Site Core`, `Stages And Progress`?**
  _High betweenness centrality (0.467) - this node is a cross-community bridge._
- **Why does `renderSpeak()` connect `Practice: Speak, Dictation, Ear` to `Library And Resources`, `Placement Test Scoring`, `Shell, Language And Accent`?**
  _High betweenness centrality (0.229) - this node is a cross-community bridge._