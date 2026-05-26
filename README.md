# Machine Learning Handbook

An interactive, single-file study guide covering the core concepts of machine learning. Built for beginners and practitioners who want a rigorous but approachable reference — from first principles through ensemble methods.

## Contents

The guide is structured as a narrative arc rather than an isolated list of algorithms. Each chapter builds on the previous one.

| Chapter | Topic |
|---------|-------|
| 00 | What is Machine Learning? |
| 01 | Linear Regression |
| 02 | Logistic Regression |
| 03 | Model Evaluation |
| 04 | Overfitting and Regularization |
| 05 | Decision Trees and Random Forest |
| 06 | Distance and Similarity |
| 07 | K-Nearest Neighbors |
| 08 | Clustering |
| 09 | Naive Bayes |
| 10 | Support Vector Machines |
| 11 | Ensemble Methods |

## Features

Each chapter includes four sections:

- **Deep Dive** — Detailed explanations with real-world intuition before the math
- **Key Points** — Condensed reference cards for quick review
- **Practice Quiz** — 8 questions per chapter with scored feedback and explanations
- **Coding** — In-browser Python challenges that run without any setup

All coding challenges execute directly in the browser via [Skulpt](https://skulpt.org). No installation, no server, no dependencies.

## Usage

Download `index.html` and open it in any modern browser. That is the entire application.

Alternatively, serve it with any static file server:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000` in your browser.

## Design Decisions

**Single file.** Everything — HTML, CSS, JavaScript, and all content — lives in one file. No build step, no framework, no network requests at runtime (beyond loading fonts and CodeMirror from CDN on first load).

**No backend.** Code execution uses Skulpt, a Python-to-JavaScript compiler. This means pure Python only — no NumPy, Pandas, or scikit-learn. All challenges are implemented from scratch, which is intentional: building KNN or K-Means by hand is a better learning exercise than calling `.fit()`.

**Narrative ordering.** Topics are sequenced so each chapter provides context for the next. Model Evaluation (Ch. 03) comes immediately after seeing two algorithms — so the question "but is it any good?" feels real. Overfitting (Ch. 04) is covered before introducing additional algorithms, so every algorithm after it is taught with that lens already in place.

## Browser Compatibility

Tested in Chrome, Firefox, Safari, and Edge. Requires JavaScript enabled. Mobile-responsive with a collapsible sidebar.

## Contributing

Content corrections, additional quiz questions, and improved coding challenges are welcome. Open an issue or submit a pull request.

For structural changes to chapters or the addition of new topics, please open an issue first to discuss the approach.
