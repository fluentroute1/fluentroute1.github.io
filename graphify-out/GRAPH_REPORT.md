# Graph Report - fluent-route  (2026-11-04)

## Corpus Check
- Corpus is ~14,721 words - fits in a single context window. You may not need a graph.

## Summary
- 82 nodes · 126 edges · 8 communities
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Practice
- Flashcards
- Placement Test Scoring
- Sign-in And Sync
- Characters And Lip Sync
- Sign-in And Sync
- Personal Map And Lessons
- Stages And Progress

## God Nodes (most connected - your core abstractions)
1. `renderTest()` - 19 edges
2. `renderSpeak()` - 10 edges
3. `renderAll()` - 9 edges
4. `say() + accentVoices()/vScore(): clearest voice of the chosen accent only (Natural > Google > local), natural pitch` - 8 edges
5. `finishTest()` - 8 edges
6. `renderShell() header + nav` - 8 edges
7. `Accent choice accentPick() in Practice, test and tips (not in header)` - 7 edges
8. `renderHome() app-style landing (hero with talking characters, features, route, steps)` - 7 edges
9. `Google sign-in + sync: Firebase project fluent-route-ed587 (europe-west1), users/{uid} doc, Sign in / Sign up button; auth change redraws the open screen` - 7 edges
10. `renderToday()` - 6 edges

## Surprising Connections (you probably didn't know these)
- `renderMore() library + tips` --calls--> `Accent choice accentPick() in Practice, test and tips (not in header)`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 1_
- `renderShell() header + nav` --shares_data_with--> `Accent choice accentPick() in Practice, test and tips (not in header)`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 5_
- `renderTest()` --calls--> `Accent choice accentPick() in Practice, test and tips (not in header)`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 4_
- `selfCheck() scoring asserts` --calls--> `matchWords() LCS word match`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 2_
- `renderHome() app-style landing (hero with talking characters, features, route, steps)` --calls--> `say() + accentVoices()/vScore(): clearest voice of the chosen accent only (Natural > Google > local), natural pitch`  [EXTRACTED]
  index.html → index.html  _Bridges community 0 → community 3_

## Import Cycles
- None detected.

## Communities (8 total, 0 thin omitted)

### Community 0 - "Practice"
Cohesion: 0.20
Nodes (14): Accent choice accentPick() in Practice, test and tips (not in header), Dictation practice (dictPool, dCheck), Ear training minimal pairs (EAR, newEar), High-variability phonetic training, listen() speech recognition, LISTEN listening item bank, matchWords() LCS word match, micMsg() mic errors (+6 more)

### Community 1 - "Flashcards"
Cohesion: 0.16
Nodes (15): CARDS flashcard deck, curView(): no hash always opens the landing (#home); hasProgress() switches its main button to Continue, Desktop sidebar layout (.side, .today-grid) + phone bottom bar, DRAW map + onlyIf(): only the visible screen renders, dueCards(), grade() Leitner scheduler, Leitner spaced repetition, NEW_PER_DAY = 10 new flashcards a day (+7 more)

### Community 2 - "Placement Test Scoring"
Cohesion: 0.20
Nodes (10): Computer adaptive testing, eap() ability estimate, finishTest(), overall() old 3-part score (replaced by overall6), pCorrect() item response model, pickItem() adaptive selection, selfCheck() scoring asserts, stepScore() / nextStep() adaptive passage scoring (+2 more)

### Community 3 - "Sign-in And Sync"
Cohesion: 0.20
Nodes (10): Published artifact claude.ai/artifact/67Qn5XzDPdmhtZhCMaVHUF, Fluent Route site, Fonts: Baloo Bhaijaan 2 + Readex Pro, Logo: route ending in speech bubble (LOGO, logo.svg), Motion switch: html.motion, motionPref(), fr-motion, renderHome() app-style landing (hero with talking characters, features, route, steps), ROUTE_SVG: illustrated landscape route with drawing road and flag, SEO head: meta, Open Graph, JSON-LD, canonical (+2 more)

### Community 4 - "Characters And Lip Sync"
Cohesion: 0.24
Nodes (10): CANDO level descriptors, CHARS + charSVG(): illustrated 2D Emma (wavy bob + clip), Jack, Sara, Leo with 8 mouth visemes, CTESTS word-completion passages A2-C2, DIALOGS conversation bank (12), Lip sync + life engine: VISEME, visemesFor, lipWord, lipLine, lookAt gaze, random blinks and glances, playLines() + voiceFor() + voiceGender(): voice always matches the character gender, distinct voice per character, word-boundary lip sync, renderTest(), Test mistakes review (tst.wrong) (+2 more)

### Community 5 - "Sign-in And Sync"
Cohesion: 0.31
Nodes (9): Google sign-in + sync: Firebase project fluent-route-ed587 (europe-west1), users/{uid} doc, Sign in / Sign up button; auth change redraws the open screen, currentStage(), Arabic/English switch (S.lang, L(), tx()), place (placement result), renderShell() header + nav, firestore.rules: users/{uid} owner only, stageDone(), store (localStorage wrapper) (+1 more)

### Community 6 - "Personal Map And Lessons"
Cohesion: 0.29
Nodes (7): buildMap(): personal map from test result, boost chapter for weak skills, weak skills first, GRAMMAR: 30 lessons A1-C2 (Arabic explanation, examples, quiz), mapHTML() + drawMapPath(): illustrated winding lesson path, overall6() weighted six-part level, renderPath(), openSheet() lesson sheet: grammar quiz, vocab, listening, speaking, pronunciation, reading, writing, VOCAB_SETS + WRITING tasks per level

### Community 7 - "Stages And Progress"
Cohesion: 0.50
Nodes (4): CEFR levels, LV levels A1-Native, STAGES with checklists, UOE grammar and reading item bank

## Knowledge Gaps
- **25 isolated node(s):** `micMsg() mic errors`, `PROMPTS free-talk topics`, `High-variability phonetic training`, `Shadowing`, `curView(): no hash always opens the landing (#home); hasProgress() switches its main button to Continue` (+20 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 28 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `renderTest()` connect `Characters And Lip Sync` to `Practice`, `Flashcards`, `Placement Test Scoring`, `Sign-in And Sync`, `Personal Map And Lessons`, `Stages And Progress`?**
  _High betweenness centrality (0.519) - this node is a cross-community bridge._
- **What connects `micMsg() mic errors`, `PROMPTS free-talk topics`, `High-variability phonetic training` to the rest of the system?**
  _25 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Why does `renderAll()` connect `Flashcards` to `Practice`, `Sign-in And Sync`, `Characters And Lip Sync`, `Sign-in And Sync`, `Personal Map And Lessons`?**
  _High betweenness centrality (0.306) - this node is a cross-community bridge._
- **Why does `finishTest()` connect `Placement Test Scoring` to `Characters And Lip Sync`, `Personal Map And Lessons`?**
  _High betweenness centrality (0.145) - this node is a cross-community bridge._