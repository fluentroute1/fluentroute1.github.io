# Graph Report - fluent-route  (2026-11-04)

## Corpus Check
- Corpus is ~7,542 words - fits in a single context window. You may not need a graph.

## Summary
- 58 nodes · 84 edges · 8 communities
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Practice: Speak, Dictation, Ear
- Layout And Shell
- Logo, SEO And Fonts
- Flashcards
- Placement Test Scoring
- Site Core
- Site Core
- Stages And Progress

## God Nodes (most connected - your core abstractions)
1. `renderTest()` - 12 edges
2. `renderSpeak()` - 10 edges
3. `renderAll()` - 9 edges
4. `say() accent-aware speech` - 6 edges
5. `Accent choice accentPick() in Practice, test and tips (not in header)` - 6 edges
6. `renderShell() header + nav` - 6 edges
7. `renderMore() library + tips` - 5 edges
8. `renderToday()` - 5 edges
9. `Dictation practice (dictPool, dCheck)` - 5 edges
10. `Fluent Route site` - 5 edges

## Surprising Connections (you probably didn't know these)
- `Fluent Route site` --references--> `renderAll()`  [EXTRACTED]
  index.html → index.html  _Bridges community 1 → community 2_
- `renderAll()` --calls--> `renderSpeak()`  [EXTRACTED]
  index.html → index.html  _Bridges community 1 → community 0_
- `renderAll()` --calls--> `renderTest()`  [EXTRACTED]
  index.html → index.html  _Bridges community 1 → community 6_
- `renderAll()` --calls--> `renderWords()`  [EXTRACTED]
  index.html → index.html  _Bridges community 1 → community 3_
- `stageDone()` --shares_data_with--> `STAGES with checklists`  [EXTRACTED]
  index.html → index.html  _Bridges community 1 → community 7_

## Import Cycles
- None detected.

## Communities (8 total, 0 thin omitted)

### Community 0 - "Practice: Speak, Dictation, Ear"
Cohesion: 0.22
Nodes (12): Accent choice accentPick() in Practice, test and tips (not in header), Dictation practice (dictPool, dCheck), Ear training minimal pairs (EAR, newEar), High-variability phonetic training, listen() speech recognition, LISTEN listening item bank, micMsg() mic errors, PROMPTS free-talk topics (+4 more)

### Community 1 - "Layout And Shell"
Cohesion: 0.23
Nodes (12): currentStage(), Desktop sidebar layout (.side, .today-grid) + phone bottom bar, Arabic/English switch (S.lang, L(), tx()), renderAll(), renderMore() library + tips, renderPath(), renderShell() header + nav, renderToday() (+4 more)

### Community 2 - "Logo, SEO And Fonts"
Cohesion: 0.29
Nodes (7): Published artifact claude.ai/artifact/67Qn5XzDPdmhtZhCMaVHUF, Fluent Route site, Fonts: Baloo Bhaijaan 2 + Readex Pro, Logo: route ending in speech bubble (LOGO, logo.svg), Animations (rise, stagger, flip, pulse, pop), SEO head: meta, Open Graph, JSON-LD, canonical, robots.txt, sitemap.xml, site.webmanifest, og.png, icons

### Community 3 - "Flashcards"
Cohesion: 0.29
Nodes (7): CARDS flashcard deck, dueCards(), grade() Leitner scheduler, Leitner spaced repetition, place (placement result), renderWords(), store (localStorage wrapper)

### Community 4 - "Placement Test Scoring"
Cohesion: 0.40
Nodes (6): Computer adaptive testing, eap() ability estimate, matchWords() LCS word match, pCorrect() item response model, pickItem() adaptive selection, selfCheck() scoring asserts

### Community 5 - "Site Core"
Cohesion: 0.40
Nodes (4): finishTest(), overall() weighted level + confidence, vocabScore() Milton bands, X_Lex vocabulary size method

### Community 6 - "Site Core"
Cohesion: 0.50
Nodes (4): CANDO level descriptors, renderTest(), Test mistakes review (tst.wrong), VOCAB X_Lex word list with fake words

### Community 7 - "Stages And Progress"
Cohesion: 0.50
Nodes (4): CEFR levels, LV levels A1-Native, STAGES with checklists, UOE grammar and reading item bank

## Knowledge Gaps
- **17 isolated node(s):** `route() hash router`, `USUK word table`, `PROMPTS free-talk topics`, `High-variability phonetic training`, `Shadowing` (+12 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 19 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `renderTest()` connect `Site Core` to `Practice: Speak, Dictation, Ear`, `Layout And Shell`, `Flashcards`, `Placement Test Scoring`, `Site Core`, `Stages And Progress`?**
  _High betweenness centrality (0.474) - this node is a cross-community bridge._
- **What connects `route() hash router`, `USUK word table`, `PROMPTS free-talk topics` to the rest of the system?**
  _17 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Why does `renderAll()` connect `Layout And Shell` to `Practice: Speak, Dictation, Ear`, `Logo, SEO And Fonts`, `Flashcards`, `Site Core`?**
  _High betweenness centrality (0.438) - this node is a cross-community bridge._
- **Why does `renderSpeak()` connect `Practice: Speak, Dictation, Ear` to `Layout And Shell`, `Placement Test Scoring`?**
  _High betweenness centrality (0.204) - this node is a cross-community bridge._