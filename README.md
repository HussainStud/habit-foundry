# Habit Foundry

A factory-builder habit tracker. Each plot is a habit "production line": the extractor mines a unit worth 1, every machine multiplies it, and each machine grows 1% stronger on every day you run it. Missed days cost nothing.

## Run

It's a single self-contained page — open `index.html` in a browser, or serve it:

```sh
python3 -m http.server 8000
```

## Storage

When hosted as a Claude artifact, progress saves privately to your Claude account (`window.claude` db). Anywhere else it falls back to `localStorage` in the browser.
