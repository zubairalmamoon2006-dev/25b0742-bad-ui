# 🔋 Creatively Bad Battery Indicator

## Concept

A parody of a system battery preferences panel that takes a simple "check your battery percentage" task and turns it into a soul-crushing 6-step ordeal.

### The Bad UI Patterns Used

1. **Unnecessary CAPTCHA** — You must verify you're human before viewing your own battery. Deliberately broken so it takes 5 attempts.

2. **Fake diagnostic** — A theatrical progress bar with nonsense messages ("Consulting battery horoscope...", "Negotiating with electrons...") that wastes 10+ seconds for no reason.

3. **Terms of viewing agreement** — You must "legally agree" that looking at the battery drains it faster.

4. **Conflicting gauges** — Three gauges show different values (Optimistic %, Pessimistic %, and "Real Battery %" which is always `??`).

5. **Battery drains while you watch** — The percentage fluctuates and gradually decreases just from observing the dashboard.

6. **"Turbo Boost"** — Labelled as a performance enhancer, it actually rapidly drains the battery to zero.

7. **Fake calibration** — A progress bar that takes 20+ seconds and resets the battery to a random value.

8. **Premium upsell** — "Unlock accurate readings" modal that does nothing when dismissed.

9. **Comic Sans** everywhere for that "system preference" feel.

10. **Passive-aggressive microcopy** — "Your battery is doing its best. That's what matters."

### Technical Execution

- Static HTML/CSS/JS — no frameworks, no build tools.
- Works by opening `index.html` directly in a browser.
- 6-step wizard flow with animated transitions.
- Real-time battery fluctuation via `setInterval`.
- CSS-only animations for the diagnostic bar and premium button glow.

### Files

| File | Purpose |
|------|---------|
| `index.html` | Structure with fake OS chrome and 6-step wizard |
| `style.css` | All styles — Comic Sans, gradients, animations |
| `script.js` | All interactivity — CAPTCHA, diagnostic, fluctuation, drain |
| `README.md` | This design document |
