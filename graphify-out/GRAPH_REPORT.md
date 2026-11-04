# Graph Report - fluent-route  (2026-11-04)

## Corpus Check
- Corpus is ~10,303 words - fits in a single context window. You may not need a graph.

## Summary
- 71 nodes · 105 edges · 7 communities
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Practice
- Sign-in And Sync
- Placement Test Scoring
- Flashcards
- Placement Test Scoring
- Site Core
- Stages And Progress

## God Nodes (most connected - your core abstractions)
1. `renderTest()` - 16 edges
2. `renderSpeak()` - 10 edges
3. `renderAll()` - 9 edges
4. `renderShell() header + nav` - 8 edges
5. `finishTest()` - 8 edges
6. `say() accent-aware speech` - 7 edges
7. `Accent choice accentPick() in Practice, test and tips (not in header)` - 6 edges
8. `renderToday()` - 6 edges
9. `Dictation practice (dictPool, dCheck)` - 5 edges
10. `renderMore() library + tips` - 5 edges

## Surprising Connections (you probably didn't know these)
- `renderShell() header + nav` --shares_data_with--> `Accent choice accentPick() in Practice, test and tips (not in header)`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 1_
- `renderTest()` --calls--> `Accent choice accentPick() in Practice, test and tips (not in header)`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 2_
- `renderAll()` --calls--> `renderMore() library + tips`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 3_
- `renderShell() header + nav` --calls--> `currentStage()`  [EXTRACTED]
  index.html → index.html  _Bridges community 3 → community 1_
- `renderToday()` --calls--> `dueCards()`  [EXTRACTED]
  index.html → index.html  _Bridges community 5 → community 3_

## Import Cycles
- None detected.

## Communities (7 total, 0 thin omitted)

### Community 0 - "Practice"
Cohesion: 0.19
Nodes (14): Accent choice accentPick() in Practice, test and tips (not in header), Dictation practice (dictPool, dCheck), Ear training minimal pairs (EAR, newEar), High-variability phonetic training, listen() speech recognition, LISTEN listening item bank, micMsg() mic errors, PROMPTS free-talk topics (+6 more)

### Community 1 - "Sign-in And Sync"
Cohesion: 0.16
Nodes (14): Published artifact claude.ai/artifact/67Qn5XzDPdmhtZhCMaVHUF, Google sign-in: fbInit, signIn, pullCloud, pushCloud (Firebase, config empty until set), CHARS + charSVG(): Emma, Jack, Sara, Leo characters, Desktop sidebar layout (.side, .today-grid) + phone bottom bar, Fluent Route site, Fonts: Baloo Bhaijaan 2 + Readex Pro, Logo: route ending in speech bubble (LOGO, logo.svg), Motion switch: html.motion, motionPref(), fr-motion (+6 more)

### Community 2 - "Placement Test Scoring"
Cohesion: 0.20
Nodes (12): CANDO level descriptors, Computer adaptive testing, CTESTS word-completion passages A2-C2, DIALOGS conversation bank (12), eap() ability estimate, matchWords() LCS word match, pCorrect() item response model, pickItem() adaptive selection (+4 more)

### Community 3 - "Flashcards"
Cohesion: 0.20
Nodes (12): currentStage(), curView() / hasProgress(): new visitors land on #home, DRAW map + onlyIf(): only the visible screen renders, grade() Leitner scheduler, Leitner spaced repetition, renderAll(), renderPath(), renderToday() (+4 more)

### Community 4 - "Placement Test Scoring"
Cohesion: 0.25
Nodes (6): finishTest(), overall() old 3-part score (replaced by overall6), overall6() weighted six-part level, stepScore() / nextStep() adaptive passage scoring, vocabScore() Milton bands, X_Lex vocabulary size method

### Community 5 - "Site Core"
Cohesion: 0.33
Nodes (6): CARDS flashcard deck, dueCards(), Arabic/English switch (S.lang, L(), tx()), NEW_PER_DAY = 10 new flashcards a day, place (placement result), store (localStorage wrapper)

### Community 6 - "Stages And Progress"
Cohesion: 0.50
Nodes (4): CEFR levels, LV levels A1-Native, STAGES with checklists, UOE grammar and reading item bank

## Knowledge Gaps
- **23 isolated node(s):** `micMsg() mic errors`, `PROMPTS free-talk topics`, `USUK word table`, `High-variability phonetic training`, `Shadowing` (+18 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 26 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `renderTest()` connect `Placement Test Scoring` to `Practice`, `Sign-in And Sync`, `Flashcards`, `Placement Test Scoring`, `Site Core`, `Stages And Progress`?**
  _High betweenness centrality (0.526) - this node is a cross-community bridge._
- **What connects `micMsg() mic errors`, `PROMPTS free-talk topics`, `USUK word table` to the rest of the system?**
  _23 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Why does `renderAll()` connect `Flashcards` to `Practice`, `Sign-in And Sync`, `Placement Test Scoring`?**
  _High betweenness centrality (0.347) - this node is a cross-community bridge._
- **Why does `finishTest()` connect `Placement Test Scoring` to `Placement Test Scoring`?**
  _High betweenness centrality (0.181) - this node is a cross-community bridge._