# Macro Tracker

A browser-based macro tracker for logging meal photos, estimating macros, and saving a daily log.

## Features

- Upload a meal photo and preview it in the app.
- Estimate calories, protein, carbs, fat, sugar, and saturated fat from the filename or food hint.
- Pick the meal or beverage slot and serving size before adding to the daily log.
- Show each logged food item name under its meal group.
- Edit or delete individual logged food entries without clearing the whole meal.
- Track daily totals by date against fixed macro targets: 90g protein, 209g carbs, 45g fat, less than 42g sugar, less than 18g saturated fat, and less than 1568 calories.
- Store entries in browser local storage.

## Deployment

This repository is configured for GitHub Pages through `.github/workflows/deploy.yml`.

The current estimator is intentionally lightweight. It does not perform real computer vision. Known foods and common beverages use local keyword estimates; unknown foods search Open Food Facts first, then USDA FoodData Central using its public API demo key.