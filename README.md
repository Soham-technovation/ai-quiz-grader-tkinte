# AI Quiz Grader (Tkinter)

A lightweight desktop tool that grades multiple-choice (MCQ) answers via a Tkinter GUI, provides detailed per-question feedback, and lets instructors edit the answer key at runtime (JSON-backed). An optional Linear Regression predictor estimates expected score from prior attempts.

## Features

- **Runtime‑editable answer key** (menu → Answer Key → Edit…, persisted to JSON).
- Accept per-question entries or pasted answer text (e.g., Q1:A, 2 b).
- **One‑click grading** with Correct/Wrong/Not Answered feedback.
- **History-based score predictor** (simple y = m x + b linear model).
- Zero external services and no OCR dependencies.

## Quick start

- Python 3.10+
- Optional predictor: `pip install -r requirements.txt`
- Run:
  ```
  python ai_quiz_grader_runtime_key.py
  ```

## Usage

- Enter answers or paste in the text box, then click Grade.
- Edit the answer key from the menu and Save; the UI rebuilds automatically.
- After at least two attempts, open the predictor panel, click Train & Predict, and view coefficients and the score estimate.

## Files

- `ai_quiz_grader_runtime_key.py` — main app.
- `answer_key.json` — sample answer key (generated on first save if missing).
- `docs/report-main-body.md` — ready-to-use main body for your academic report.
- `docs/teachers-remarks.md` — printable rubric for evaluation.

## Screenshots

Add UI screenshots in `docs/screenshots`.

## License

MIT — see LICENSE.
