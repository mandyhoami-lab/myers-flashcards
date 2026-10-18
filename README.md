# myers-flashcards

170 vocab flashcards for Myers Experimental Psychology (chapters 1–16), running on a zero-dependency flashcard engine. The live deck is at [amandata.dev/learn](https://amandata.dev/learn).

## Files

- `index.html` — the full Myers deck, ready to study. Open it and flip.
- `flashcards.js` — the engine: renders the deck, tag filter, shuffle, missed-only drill, progress bar, click/space flip, arrow-key grading (`←` still learning, `→` got it), done screen. Any page sets `window.FLASHCARD_DECK` before loading it:
  ```js
  window.FLASHCARD_DECK = {
    title: 'My deck',
    sub: '12 terms · tap a card to flip',
    cards: [{ tag: 'Topic', term: 'Front', def: 'Back' }]
  };
  ```
- `flashcards.css` — pixel-art styling, themeable via CSS variables (`--ink`, `--dim`, `--line`, `--card-bg`, `--tag`, …). Ships with dark-theme defaults.

## Use it

Swap in your own deck object and drop the three files anywhere static. No build step, no framework.

Built by [Mandy](https://amandata.dev) for PSY 410.
