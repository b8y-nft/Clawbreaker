# 🦞 CLAWBREAKER — $CLAWD Arcade

> A lobster-themed Breakout clone with a micro $CLAWD token economy. Break bricks, earn $CLAWD, cash out before you lose your lives — or lose everything.

**[▶ PLAY NOW](https://yourusername.github.io/clawbreaker)**

---

## What is this?

CLAWBREAKER is a proof-of-concept arcade game built around the $CLAWD token ecosystem. It's a single HTML file — no installs, no downloads, plays entirely in your browser.

### The Loop
- Pay a 0.5 $CLAWD buy-in to play
- Break bricks to earn micro $CLAWD rewards (0.001 – 0.05 per brick)
- Cash out any time you still have lives to lock in your earnings
- Lose all 3 lives and your $CLAWD goes to zero
- One game per day — your lobster needs rest

### Why once per day?
Scarcity creates value. A daily play limit makes each session feel meaningful, builds a return habit, and prevents reward farming.

---

## Brick Types

| Brick | Reward | Effect |
|-------|--------|--------|
| 🪸 Coral | 0.001 | Standard |
| ⭐ Starfish | 0.005 | Standard |
| 🦀 Crab | 0.008 | 2 hits to break |
| 📦 Treasure | 0.025 | 2 hits, rare |
| 💨 Dud Mine | 0.002 | Weird bounce, no life lost |
| 💨 Smoke Mine | 0.003 | Fogs the screen briefly |
| 🧊 Slow Mine | 0.004 | Halves ball speed |
| ☢️ Live Mine | 0.015 | Costs a life — rare but dangerous |

---

## Sticky Mechanics

- **Daily streak bonus** — play consecutive days to earn up to 2× rewards
- **Streak multiplier** — 5 hits in a row = 2×, 10 in a row = 3×
- **Milestones** — celebration popups at 0.01, 0.025, 0.05, 0.1, 0.25 $CLAWD
- **Local leaderboard** — top 5 personal sessions tracked
- **"So close" death screen** — shows exactly how far you were from the next milestone
- **Power-ups** — wide claw, multi-bubble, slow tide, shield

---

## Bot Resistance

- Pre-game lobster CAPTCHA (click only the 🦞)
- Canvas + screen + timezone fingerprint for daily session lock
- Per-session random ball drift so hardcoded trajectories fail
- Invisible honeypot element — triggers instant game over if hit programmatically

---

## Status

This is a **proof of concept**. The $CLAWD rewards are simulated locally — no real token transfers happen in this version. The dApp roadmap includes:

- [ ] Wallet connect (Rainbow/MetaMask)
- [ ] On-chain burn on buy-in
- [ ] Smart contract cashout verification
- [ ] Server-side game state validation
- [ ] Global leaderboard

---

## Run Locally

No build step needed. Just open the file:

```bash
git clone https://github.com/yourusername/clawbreaker
open clawbreaker/index.html
```

Or drag `index.html` into any browser.

---

## Controls

| Input | Action |
|-------|--------|
| Mouse / Touch | Move paddle |
| Arrow keys / WASD | Move paddle |
| Space / Tap | Launch ball |
| Cash Out button | Lock in your $CLAWD |

---

## Built With

Vanilla JS + HTML5 Canvas. No libraries. No frameworks. One file.

---

*Part of the $CLAWD / OpenClaw ecosystem.*
