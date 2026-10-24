# Project State: my-first-game

- **Current Version:** v1.0 - Full rebuild
- **Goal:** Carolina Panthers trivia game (embedded in the Arcade tab of car-panther-site)
- **Status:** Live on Vercel (https://my-first-game-opal.vercel.app)

## What's in it
- 67 fact-checked questions in 4 categories (History, Legends, 2026 Squad, Stadium) and 3 difficulty levels.
- Modes: Classic (10 questions, 15 s each), Blitz (60 s, misses cost 3 s), Sudden Death (gets harder, one miss ends it), Daily Challenge (same 5 questions for everyone each day, one attempt).
- Scoring: 100 per correct answer + up to 50 speed bonus, multiplied by a streak bonus (up to +50%).
- Lifelines: 50/50 and Skip, once per game (not in the Daily Challenge).
- Results: rank, accuracy, best streak, emoji grid, Share button, review of missed questions, personal bests saved in the browser.
- Keyboard: 1-4 to answer, Enter for next.

## Editing questions
Questions live in the `QUESTIONS` array near the top of the script in `index.html`. The first answer in each `a` list is the correct one (answers are shuffled on screen). Add a `fact` so players learn something either way.

## Acceptance Test
- Open `index.html`. Play each mode once.
- Classic: answer with keys 1-4, use 50/50 and Skip, let one timer run out, check the review list.
- Daily: finish it, reload, confirm it shows "Done today" and can't be replayed.
