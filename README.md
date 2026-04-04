# MiniGames

A growing collection of mobile-first browser mini-games, wrapped in a PWA shell for easy home screen installation.

## Games

### Neon Flow
Connect matching colored dots on a grid by drawing paths between them. Every cell must be filled to solve the puzzle. Puzzles are procedurally generated and guaranteed to be solvable.

### Gemstone Mania
A match-3 puzzle game. Swap adjacent gems to form rows or columns of three or more matching stones. Gems fall to fill the gaps and new ones drop in from the top.

## PWA

The shell can be installed as a standalone app on Android (Chrome → "Add to Home Screen") and iOS (Safari → Share → "Add to Home Screen"). Games are cached for offline play after the first visit.

## Structure

```
index.html              — game launcher (PWA shell)
manifest.json           — PWA manifest
sw.js                   — service worker (network-first, 3s timeout, cache fallback)
icons/icon.svg          — app icon
flow-logic/             — Neon Flow game
gemstone-mania/         — Gemstone Mania game
```
