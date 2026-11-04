# Graph Report - fluent-route  (2026-11-04)

## Corpus Check
- Corpus is ~11,121 words - fits in a single context window. You may not need a graph.

## Summary
- 74 nodes · 109 edges · 7 communities
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Practice
- Sign-in And Sync
- Placement Test Scoring
- Flashcards
- Illustrations And Characters
- Stages And Progress
- Illustrations And Characters

## God Nodes (most connected - your core abstractions)
1. `renderTest()` - 17 edges
2. `renderSpeak()` - 10 edges
3. `renderAll()` - 9 edges
4. `renderShell() header + nav` - 8 edges
5. `finishTest()` - 8 edges
6. `say() accent-aware speech` - 7 edges
7. `renderHome() app-style landing (hero with talking characters, features, route, steps)` - 7 edges
8. `Accent choice accentPick() in Practice, test and tips (not in header)` - 6 edges
9. `renderToday()` - 6 edges
10. `Dictation practice (dictPool, dCheck)` - 5 edges

## Surprising Connections (you probably didn't know these)
- `renderMore() library + tips` --calls--> `Accent choice accentPick() in Practice, test and tips (not in header)`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 3_
- `renderShell() header + nav` --shares_data_with--> `Accent choice accentPick() in Practice, test and tips (not in header)`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 1_
- `renderTest()` --calls--> `Accent choice accentPick() in Practice, test and tips (not in header)`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 4_
- `renderHome() app-style landing (hero with talking characters, features, route, steps)` --calls--> `say() accent-aware speech`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 6_
- `renderHome() app-style landing (hero with talking characters, features, route, steps)` --calls--> `Google sign-in + sync: Firebase project fluent-route-ed587 (europe-west1), users/{uid} doc, Sign in / Sign up button`  [EXTRACTED]
  index.html → index.html  _Bridges community 1 → community 6_

## Import Cycles
- None detected.

## Communities (7 total, 0 thin omitted)

### Community 0 - "Practice"
Cohesion: 0.23
Nodes (12): Accent choice accentPick() in Practice, test and tips (not in header), Dictation practice (dictPool, dCheck), Ear training minimal pairs (EAR, newEar), High-variability phonetic training, listen() speech recognition, matchWords() LCS word match, micMsg() mic errors, PROMPTS free-talk topics (+4 more)

### Community 1 - "Sign-in And Sync"
Cohesion: 0.18
Nodes (13): Published artifact claude.ai/artifact/67Qn5XzDPdmhtZhCMaVHUF, Google sign-in + sync: Firebase project fluent-route-ed587 (europe-west1), users/{uid} doc, Sign in / Sign up button, Fluent Route site, Fonts: Baloo Bhaijaan 2 + Readex Pro, Arabic/English switch (S.lang, L(), tx()), Logo: route ending in speech bubble (LOGO, logo.svg), Motion switch: html.motion, motionPref(), fr-motion, place (placement result) (+5 more)

### Community 2 - "Placement Test Scoring"
Cohesion: 0.18
Nodes (11): Computer adaptive testing, eap() ability estimate, finishTest(), overall() old 3-part score (replaced by overall6), overall6() weighted six-part level, pCorrect() item response model, pickItem() adaptive selection, selfCheck() scoring asserts (+3 more)

### Community 3 - "Flashcards"
Cohesion: 0.20
Nodes (12): CARDS flashcard deck, Desktop sidebar layout (.side, .today-grid) + phone bottom bar, dueCards(), grade() Leitner scheduler, Leitner spaced repetition, NEW_PER_DAY = 10 new flashcards a day, renderAll(), renderMore() library + tips (+4 more)

### Community 4 - "Illustrations And Characters"
Cohesion: 0.22
Nodes (10): CANDO level descriptors, CHARS + charSVG(): illustrated 2D Emma, Jack, Sara, Leo (outlines, shading, 3 mouth shapes, idle + talk animation), CTESTS word-completion passages A2-C2, DIALOGS conversation bank (12), LISTEN listening item bank, playLines() + voiceFor() + mouthLoop(): named speakers with own voices and moving mouths, renderTest(), Test mistakes review (tst.wrong) (+2 more)

### Community 5 - "Stages And Progress"
Cohesion: 0.29
Nodes (7): CEFR levels, currentStage(), LV levels A1-Native, renderPath(), stageDone(), STAGES with checklists, UOE grammar and reading item bank

### Community 6 - "Illustrations And Characters"
Cohesion: 0.33
Nodes (6): curView() / hasProgress(): new visitors land on #home, DRAW map + onlyIf(): only the visible screen renders, renderHome() app-style landing (hero with talking characters, features, route, steps), route() hash router, ROUTE_SVG: illustrated landscape route with drawing road and flag, SPOT: illustrated feature-card drawings

## Knowledge Gaps
- **24 isolated node(s):** `micMsg() mic errors`, `PROMPTS free-talk topics`, `USUK word table`, `High-variability phonetic training`, `Shadowing` (+19 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 27 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `renderTest()` connect `Illustrations And Characters` to `Practice`, `Sign-in And Sync`, `Placement Test Scoring`, `Flashcards`, `Stages And Progress`, `Illustrations And Characters`?**
  _High betweenness centrality (0.531) - this node is a cross-community bridge._
- **What connects `micMsg() mic errors`, `PROMPTS free-talk topics`, `USUK word table` to the rest of the system?**
  _24 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Why does `renderAll()` connect `Flashcards` to `Practice`, `Sign-in And Sync`, `Illustrations And Characters`, `Stages And Progress`, `Illustrations And Characters`?**
  _High betweenness centrality (0.330) - this node is a cross-community bridge._
- **Why does `finishTest()` connect `Placement Test Scoring` to `Illustrations And Characters`?**
  _High betweenness centrality (0.174) - this node is a cross-community bridge._