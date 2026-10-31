# Brain Battle — starter prototype

A responsive React + TypeScript browser prototype for the Brain Battle trivia game.

## Requirements
- Node.js 20 or newer
- npm

## Run locally
```bash
npm install
npm run dev
```

Open the local URL printed by Vite.

## Production build
```bash
npm run build
npm run preview
```

## What's included
- Responsive arcade-style home screen
- Ten-question local demo flow
- Multiple-choice and true/false question rendering
- 10-second timer
- Base, speed and streak scoring
- Double Points and Extra Time prototype power-ups
- Answer reveal, fun facts and results screen
- Typed question model and isolated scoring function

## Important prototype boundaries
This is the first playable frontend milestone, not the complete online game. It currently runs a local single-player demo. Public matchmaking, private rooms, WebSocket server authority, real account authentication, cloud persistence, friends, purchases, ads, production moderation, and licensed image-question content still need backend and product integration.

The score calculator in `src/game/scoring.ts` is shared-domain logic for prototyping only. In production, the authoritative copy must run on the server and the client must never be trusted to submit its own score or elapsed time.

## Next engineering milestones
1. Add automated unit tests for scoring and round state.
2. Add backend API and PostgreSQL schema.
3. Add Redis-backed room state and WebSocket matchmaking.
4. Move timer, answers, power-ups and score adjudication to the server.
5. Add account, guest migration, profiles and progression.
6. Add moderation, leaderboards, payments, rewarded ads and deployment.
