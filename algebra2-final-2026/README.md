# Honors Algebra II — Final Exam Practice Cards

Web-based flashcard practice for the **May 11, 2026** Honors Algebra II final exam (APIS, Ms. Bertiz).

Covers Chapters 5–8 of *Pearson Algebra II Common Core*:

| Ch | Topic | # Cards |
|----|-------|---------|
| 5 | Polynomial Functions (classify, end behavior, factor, divide, Pascal) | 9 |
| 6 | Radicals & Rational Exponents (nth roots, simplify, rationalize, solve, functions, inverses) | 11 |
| 7 | Exponential & Logarithmic Functions (compounding, log form, properties, equations) | 7 |
| 8 | Rational Functions (asymptotes, simplify, ×/÷, +/−, equations) | 5 |
| **Total** | | **32** |

## How to use

### Local
Open `index.html` in any modern browser:
```bash
open cards/algebra2-final-2026/index.html
```

### Online (GitHub Pages)
Push this folder to a GitHub repo, enable Pages on the `master` branch, and visit:
```
https://<your-username>.github.io/<repo-name>/cards/algebra2-final-2026/
```

## Features

- **Random card selection** — every session draws a different subset, so each student sees different problems
- **Filter by chapter** — drill on a single chapter or mix all four
- **Adjustable count** — 5 to 32 cards per session
- **Instant feedback** — pick an answer, see explanation immediately
- **Score breakdown** — per-chapter performance at session end
- **MathJax** — full LaTeX math rendering

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
  "id": "Q33",
  "chapter": "7-1",
  "topic": "Exponential growth",
  "question": "Math text with $\\LaTeX$ inline.",
  "choices": {
    "A": "first option",
    "B": "second option",
    "C": "third option",
    "D": "fourth option"
  },
  "answer": "B",
  "explanation": "Why B is correct, with $\\LaTeX$ if needed."
}
```

LaTeX uses `$...$` for inline math and `$$...$$` for display math. Backslashes inside JSON strings must be escaped (`\\frac`, `\\sqrt`, `\\cdot`, etc.).

## Source

Built from the official APIS *Final Exam Review* PDF (60 questions, Keisha Bertiz). Selected and rewritten 32 high-yield problems covering the four chapters.
