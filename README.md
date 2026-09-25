# Laya decision brain

FastAPI lab for [Laya](https://github.com/convaiinnovations/laya). The default interface is plain HTML, CSS, and JavaScript served by FastAPI, so running the demo does not require Node.js or Next.js. It lets you explore survey predictions, inspect decisions, and play Snake with Laya or take control yourself.

- App and API: http://localhost:8000
- API docs: http://localhost:8000/docs

## Run

```bash
cd backend
uv sync
uv run uvicorn main:app --reload --port 8000
```

## Survey

http://localhost:8000 — FiveThirtyEight steak & risk survey (550 respondents).

- **This person** — pick a respondent and ask Laya yes/no or A-or-B questions
- **See the math** — logits, temperature, and leave-one-out attribution for the person on the left
- **Play Snake** — ask Laya to steer or use the arrow keys / WASD; a safety check blocks reversals and unsafe moves

The previous Next.js interface remains in `frontend/` for reference.
