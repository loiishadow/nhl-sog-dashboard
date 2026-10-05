# NHL SOG Daily Dashboard

Mobile-first PWA foundation for the NHL SOG prediction project.

## Current features
- Today SOG predictions
- Next-day predictions
- Last 5 games
- FanDuel line entry and OVER/UNDER/PASS
- Frozen daily prediction snapshots
- End-of-night grading
- Local rolling learning parameters
- PWA manifest, service worker and install metadata

## Architecture direction
The current HTML remains intentionally self-contained while the project matures. The next major refactor should separate the data layer, feature engine, prediction engine, grading/learning engine and UI. That will make NHL the first sport adapter and allow NBA/NFL/MLB expansion later.

## Long-term model direction
Add play-by-play features such as even-strength/PP shot volume, shot attempts, player shot share, lineup status, PP role and opponent-specific history. Keep all pregame predictions immutable after puck drop and evaluate them against actual results.

## Native app direction
The intended native path is Expo/React Native so one TypeScript codebase can target iOS, Android and web.
