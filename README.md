# Macro Tracker

A browser-based macro tracker for logging meal photos, estimating macros, and saving a daily log.

## Features

- Upload a meal photo and preview it in the app.
- Estimate calories, protein, carbs, fat, sugar, and saturated fat from the filename or food hint.
- Pick the meal slot and serving size before adding to the daily log.
- Track daily totals by date against fixed macro targets: 90g protein, 209g carbs, 45g fat, less than 42g sugar, less than 18g saturated fat, and less than 1568 calories.
- Store entries in browser local storage.

## Deployment

This repository is configured for GitHub Pages through `.github/workflows/deploy.yml`.

The current estimator is intentionally lightweight. It does not perform real computer vision; it uses local keyword heuristics based on the photo filename and food hint.