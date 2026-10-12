# THE HUDSON PROTOCOL ✦

A six-stage, mobile-first geography scavenger hunt with **54 location riddles** and a final vault. Each stage's answers spell a secret website path using their first letters.

## Play

Open the deployed website and press **Begin the hunt**. Answer each numbered location clue, collect the first letters, then use them as the code to unlock the next chapter. There are two hints per question. Progress is saved in the player's browser.

## Deployment

This is a standalone static website with **no dependencies or build step**. The root `index.html` includes all CSS, JavaScript, and puzzle data. Import this repository in **Vercel**, choose framework **Other**, and leave the build command empty. Hash routes such as `/#/start` work without rewrites.

## Chapters and organiser answer key

| Chapter | Entry route | Result |
|---|---|---|
| The Broken Compass | `/#/start` | `SECRETGATE` |
| The Observatory | `/#/secretgate` | `MOONVAULT` |
| The Shadow Archive | `/#/moonvault` | `SHADOWKEY` |
| The Northern Signal | `/#/shadowkey` | `NORTHSTAR` |
| The Glass Labyrinth | `/#/northstar` | `FINALDOOR` |
| The Final Eight | `/#/finaldoor` | `LASTLOCK` |

Keep the organiser answer key away from the player.

## Features

- Six chapters, 54 geographic riddles, answer checking, two hints per clue and optional reveals
- Six secret paths and the final vault
- Progress autosave in localStorage and an elapsed-time clock
- Downloadable winner's certificate
- Mobile and desktop layouts, no trackers or remote libraries

## Reward and privacy

The optional Google Drive reward is intentionally **not configured**. The final vault has a joke prize and victory certificate instead. To offer a shareable prize, set `approvedRewardUrl` in the embedded `window.HUNT_DATA` inside `index.html`.

Do not publish another person's private recording without permission. Anyone can inspect the front-end source and find the answer codes, so the routes are puzzle mechanics, not real access controls. One hour is an approximate completion time, not a guarantee.
