# Honors Biology — Semester 2 Final Practice Cards

Web-based flashcard practice for the Honors Biology Semester 2 final exam (APIS).

Built from the official **Honors Biology Semester 2 Study Guide (2025–26)**.

## Coverage (32 cards across 4 sections)

| Sec | Topic | # Cards |
|-----|-------|---------|
| I  | Gene Expression & Central Dogma (transcription, translation, codons, tRNA) | 9 |
| II | Mutations (substitution, frameshift, silent, gametes, mutagens) | 6 |
| III | Genetics & Inheritance Patterns (dihybrid, linked, lethal, codominance, incomplete dominance, pedigrees) | 9 |
| IV | Variation & Adaptations (sources, types, structural/behavioral/physiological, natural/sexual selection, drift) | 8 |
| **Total** | | **32** |

## How to use

### Local
```bash
open cards/biology-semester2-2026/index.html
```

### Online (GitHub Pages)
Push this folder to a GitHub repo, enable Pages on the `master` branch, and visit:
```
https://<your-username>.github.io/<repo-name>/cards/biology-semester2-2026/
```

## Features

- **Random card selection** — every session draws a different subset, so each student sees different problems
- **Filter by section** — drill on a single topic or mix all four
- **Adjustable count** — 5 to 32 cards per session
- **Instant feedback** — pick an answer, see explanation immediately
- **Score breakdown** — per-section performance at session end

## Files

| File | Purpose |
|------|---------|
| `index.html` | Self-contained web app (HTML + CSS + JS) |
| `questions.json` | Question bank (32 questions with answers + explanations) |
| `README.md` | This file |

## Adding more questions

Edit `questions.json`. Each question follows this schema:

```json
{
  "id": "B33",
  "section": "II",
  "topic": "Chromosomal mutations",
  "question": "Question text here.",
  "choices": {
    "A": "first option",
    "B": "second option",
    "C": "third option",
    "D": "fourth option"
  },
  "answer": "B",
  "explanation": "Why B is correct."
}
```

The card UI reads `ui.categories` from the JSON to populate the section dropdown automatically — adjust those if you add a Section V or rename existing ones.

## Source

Honors Biology Semester 2 Study Guide, APIS (2025–26). Original PDF kept locally at `students/김민준/Honors_Biology_Sem2_Study_Guide_2026.pdf` (gitignored).
