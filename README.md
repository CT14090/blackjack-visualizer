# Blackjack Code Visualizer

A browser tool for COMP 202 Assignment 3 (Blackjack). Add your `blackjack.py` and
`shuffle_deck.py` to watch your own functions build and shuffle the deck, deal the
hands, play each turn and pick the winners. Errors are shown the way Python prints
them, with the line marked in a code view.

Live page: https://ct14090.github.io/blackjack-visualizer/

- Your code runs only in your own browser (Pyodide). It is never uploaded.
- The page holds no solution code. The "Handout examples" check uses only the
  examples printed in the assignment handout.

## Run it locally

Opening `index.html` directly does not work: browsers block the Python runtime on
`file://` pages. From this folder run:

```
python -m http.server 8000
```

then open http://localhost:8000.

## Files

- `index.html`: the whole tool (page, styles, scripts, and the Python harness).
- `py/`: Pyodide 0.26.4 (Python 3.12 for the browser), unchanged, plus
  `stdlib.js`, the Python standard library stored as base64 inside a script.
