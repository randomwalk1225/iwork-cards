# iWork Practice Cards

Online flashcard practice decks for iWork Math & Science Academy students.

**Live site:** https://randomwalk1225.github.io/iwork-cards/

## Decks

| Deck | Subject | Cards | Source |
|------|---------|-------|--------|
| [`algebra2-final-2026/`](algebra2-final-2026/) | Honors Algebra II — Chapters 5–8 | 32 | Pearson Algebra II Common Core |
| [`biology-semester2-2026/`](biology-semester2-2026/) | Honors Biology — Semester 2 (Genetics, Mutations, Variation) | 80 (≈4 sessions) | APIS Honors Biology Sem 2 Study Guide (2025–26) |

## How it works

Each deck is a self-contained static page:

- `index.html` — single-page card UI (vanilla JS, no build step)
- `questions.json` — question bank with answer keys and explanations
- `README.md` — deck-specific notes

A session draws a random subset from the bank, so each student sees a different mix. Pick a section to drill on a single topic, or "All" to mix everything.

## Adding a new deck

1. Make a folder `cards/<subject-name>/`
2. Create `questions.json` with the same schema as the existing decks
3. Copy or adapt `index.html` from one of the existing decks
4. Link it from the top-level `index.html`
5. Commit and push — GitHub Pages updates automatically

## License & use

Course-specific practice content for iWork Academy students. Question text and explanations are written for review purposes; source materials remain the property of their respective publishers (Pearson, APIS).
