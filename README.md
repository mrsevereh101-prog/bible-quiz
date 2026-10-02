# Bible Quiz

A single-page Bible quiz game. Everything lives in `index.html`: no build step, no dependencies beyond Google Fonts.

Open `index.html` in a browser to play, or use the published version on claude.ai.

## Quiz

Rounds of ten questions against the clock. Pick a level on the start screen:

- **Mixed:** questions from every level
- **Easy / Medium / Hard:** 100, 150 or 200 points per correct answer, plus a time bonus and a streak bonus
- **Puzzles only:** just the puzzle styles below

Answers lock in without feedback. The results screen shows your score and reviews every question with your answer, the correct one and the verse reference.

### Question styles

| Style | How it plays | Time |
|---|---|---|
| Multiple choice, True or false, Finish the verse, Who said it?, Which came first? | Pick one answer | 20s |
| Odd one out | Pick the one that doesn't belong | 20s |
| Unscramble | Tap letter tiles to spell the answer to a clue | 40s |
| Put in order | Tap items from first to last | 40s |
| Who am I? | Reveal up to three clues; each extra clue costs 25% of the points | 30s |

There are 165 questions in total (54 easy, 56 medium, 55 hard), of which 47 are puzzles. They live in the `Q` array at the top of the script; each has a level (`d`), style (`k`), question (`q`), answer, explanation (`n`) and verse reference (`r`).

## Word Fall

A falling-letter game. The letters of a Bible word drop one at a time into a 7 × 11 board. Spell any word from the word list left to right, or up and down in either direction, to clear it. Letters above fall into the gap, and new words formed that way score a chain bonus. The game ends when a letter can't enter the board.

Controls: tap a column to slide the letter there, tap its own column to drop it, or use the ◀ ⤓ ▶ buttons. On a keyboard: ← → to move, ↓ or space to drop, P or Esc to pause. The game pauses on its own when you switch away.

## Other details

- Light and dark themes follow the device setting.
- Sound effects can be switched off on the start screen; the choice is remembered.
- Best scores per level and for Word Fall are saved in the browser.
- "Copy my score" copies a one-line result to share.
