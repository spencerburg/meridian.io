# Meridian Daily

A daily geography game. Each day brings ten prompts, three in calm seas (easy), four in choppy waters (medium) and three in stormy seas (hard), such as "Name a country that borders Germany" or "Name a strait". Any correct answer counts, and rarer answers earn more leagues. Your ship sails Columbus's 1492 route from Palos to La Navidad as you score.

Everything is in `index.html`: no build step, no dependencies.

## Hosting

This repository is served by GitHub Pages from the `main` branch root. Pushing to `main` updates the site.

## Scoring on this site

Rarity is scored against a built-in estimate of how often people give each answer. Your progress, streak and stats are saved in your browser.

The version hosted on claude.ai also pools every player's answers to measure real rarity. That needs a shared database; to add one here, connect a backend such as Supabase and replace the `connect()` and `savePicks()` functions in `index.html`.
