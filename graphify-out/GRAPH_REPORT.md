# Graph Report - fluent-route  (2026-11-04)

## Corpus Check
- Corpus is ~6,676 words - fits in a single context window. You may not need a graph.

## Summary
- 49 nodes · 65 edges · 8 communities
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Flashcards
- Speaking And Mic
- Shell, Language And Accent
- Placement Test Scoring
- Site Core
- Site Core
- Stages And Progress
- Site Core

## God Nodes (most connected - your core abstractions)
1. `renderTest()` - 10 edges
2. `renderAll()` - 9 edges
3. `renderSpeak()` - 7 edges
4. `eap() ability estimate` - 5 edges
5. `finishTest()` - 5 edges
6. `selfCheck() scoring asserts` - 4 edges
7. `say() accent-aware speech` - 4 edges
8. `listen() speech recognition` - 4 edges
9. `stageDone()` - 4 edges
10. `renderShell() header + nav` - 4 edges

## Surprising Connections (you probably didn't know these)
- `Fluent Route site` --references--> `renderAll()`  [EXTRACTED]
  index.html → index.html  _Bridges community 7 → community 0_
- `renderShell() header + nav` --shares_data_with--> `US/UK accent switch (S.accent)`  [EXTRACTED]
  index.html → index.html  _Bridges community 1 → community 2_
- `CARDS flashcard deck` --shares_data_with--> `store (localStorage wrapper)`  [EXTRACTED]
  index.html → index.html  _Bridges community 2 → community 0_
- `stageDone()` --shares_data_with--> `STAGES with checklists`  [EXTRACTED]
  index.html → index.html  _Bridges community 6 → community 2_
- `renderTest()` --shares_data_with--> `UOE grammar and reading item bank`  [EXTRACTED]
  index.html → index.html  _Bridges community 6 → community 5_

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Placement test** — index_vocabscore, index_eap, index_pickitem, index_overall, index_finishtest [EXTRACTED 1.00]

## Communities (8 total, 0 thin omitted)

### Community 0 - "Flashcards"
Cohesion: 0.22
Nodes (11): CARDS flashcard deck, dueCards(), grade() Leitner scheduler, Leitner spaced repetition, renderAll(), renderMore() library + tips, renderToday(), renderWords() (+3 more)

### Community 1 - "Speaking And Mic"
Cohesion: 0.25
Nodes (8): US/UK accent switch (S.accent), listen() speech recognition, micMsg() mic errors, PROMPTS free-talk topics, renderSpeak(), say() accent-aware speech, SENTS repeat-after-me sentences, Shadowing

### Community 2 - "Shell, Language And Accent"
Cohesion: 0.33
Nodes (7): currentStage(), Arabic/English switch (S.lang, L(), tx()), place (placement result), renderPath(), renderShell() header + nav, stageDone(), store (localStorage wrapper)

### Community 3 - "Placement Test Scoring"
Cohesion: 0.40
Nodes (6): Computer adaptive testing, eap() ability estimate, matchWords() LCS word match, pCorrect() item response model, pickItem() adaptive selection, selfCheck() scoring asserts

### Community 4 - "Site Core"
Cohesion: 0.40
Nodes (4): finishTest(), overall() weighted level + confidence, vocabScore() Milton bands, X_Lex vocabulary size method

### Community 5 - "Site Core"
Cohesion: 0.50
Nodes (4): CANDO level descriptors, LISTEN listening item bank, renderTest(), VOCAB X_Lex word list with fake words

### Community 6 - "Stages And Progress"
Cohesion: 0.50
Nodes (4): CEFR levels, LV levels A1-Native, STAGES with checklists, UOE grammar and reading item bank

### Community 7 - "Site Core"
Cohesion: 0.67
Nodes (3): Published artifact claude.ai/artifact/67Qn5XzDPdmhtZhCMaVHUF, Fluent Route site, Animations (rise, stagger, flip, pulse, pop)

## Knowledge Gaps
- **16 isolated node(s):** `SENTS repeat-after-me sentences`, `PROMPTS free-talk topics`, `USUK word table`, `LISTEN listening item bank`, `VOCAB X_Lex word list with fake words` (+11 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 18 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `renderTest()` connect `Site Core` to `Flashcards`, `Speaking And Mic`, `Shell, Language And Accent`, `Placement Test Scoring`, `Site Core`, `Stages And Progress`?**
  _High betweenness centrality (0.498) - this node is a cross-community bridge._
- **What connects `SENTS repeat-after-me sentences`, `PROMPTS free-talk topics`, `USUK word table` to the rest of the system?**
  _16 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Why does `renderAll()` connect `Flashcards` to `Speaking And Mic`, `Shell, Language And Accent`, `Site Core`, `Site Core`?**
  _High betweenness centrality (0.486) - this node is a cross-community bridge._
- **Why does `renderSpeak()` connect `Speaking And Mic` to `Flashcards`, `Placement Test Scoring`?**
  _High betweenness centrality (0.233) - this node is a cross-community bridge._