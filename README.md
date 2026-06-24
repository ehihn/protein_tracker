# Protein Tracker

A minimal, single-page protein tracker that runs entirely in the browser — no build step, no dependencies, no backend. Just open `tracker.html`.

## Features

- **Tap to add** — preset foods with common protein values
- **Custom entries** — add any food with your own protein amount
- **Daily progress** — running total and progress bar against a 150g goal
- **Today's log** — see each item, remove individual entries, or reset with "New day"
- **Persistent** — saves to `localStorage` and automatically clears when the date changes
- **Dark mode** — follows your system theme via `prefers-color-scheme`
- **Installable** — works as a home-screen web app on iOS

## Usage

Download `tracker.html` and open it in any browser. On mobile, you can add it to your home screen to use it like a standalone app.

No installation, accounts, or internet connection required — all data stays in your browser's local storage.

## Customizing

The goal and preset foods are hardcoded in the `<script>` block:

- **Daily goal** — change the `GOAL` variable (default `150`).
- **Preset foods** — edit the `presets` array; each entry is `{n: "name", p: grams}`.

> Note: the preset protein values are rough estimates for convenience, not verified nutritional data. Adjust them to match the foods and portions you actually eat.

## Tech

Plain HTML, CSS, and vanilla JavaScript in a single file. No frameworks, no external requests.
