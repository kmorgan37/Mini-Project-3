# Mini Project #3 — Proposal

## What I'm Building
A quote guessing game where players read a real quote and have to guess which of two unhinged options actually said it. The twist: real people are often more unhinged than the fake options.

## Which API I'm Using
- **Kanye REST API** — https://kanye.rest (random Kanye West quotes, no key required)
- **Quotable API** — https://api.quotable.io (famous quotes from philosophers, historical figures, and public figures, no key required)
- **ZenQuotes API** — https://zenquotes.io/api (inspirational/philosophical quotes, no key required)

## Why I Chose This
I wanted to build something genuinely funny that people would want to share. The premise writes itself — real quotes from real people are often so unhinged they're impossible to tell apart from villain monologues or AI-generated nonsense. The game works because the player is always wrong in a funny way, not a frustrating way.

## Core Features
1. **Multiple game modes** — each mode pits two unlikely sources against each other (e.g. LinkedIn Post vs Supervillain, Kanye vs Philosopher, Founding Father vs Frat Boy, Deepak Chopra vs AI Nonsense)
2. **Quote display** — a real quote fetched from an API appears on screen, player picks who said it
3. **Reveal animation** — after guessing, the real answer is revealed with a reaction (shocked if wrong, smug if right)
4. **Score tracking** — running score across rounds, final roast at the end based on your results
5. **Loading + error states** — spinner while fetching, friendly message if API fails

## What I Don't Know Yet
- How async/await works with multiple API calls at once (do I fetch both at the same time or one after the other?)
- How to handle CORS issues if an API blocks browser requests
- How to structure the game state in JavaScript so switching between modes doesn't break the score
- Best way to mix real API quotes with my own hardcoded "fake" quotes in the same round