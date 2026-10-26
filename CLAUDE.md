# CLAUDE.md — Instructions for Claude Code working on this repo

You are helping Jerry (Jeremiah Guthrie), owner of Jerry's Window Cleaning,
San Diego County, improve this website + game. Keep it professional,
playable, and realistic.

## Hard rules

- Do NOT invent a fixed discount % or $ amount. Discount wording must stay:
  "Play the game, clean windows, earn a discount — call 217-552-8626 and
  mention your score to claim it."
- Business facts must stay correct: San Diego County, $110/hour regardless
  of window count, estimates 100% free, 9am-5pm 7 days a week, phone
  217-552-8626, email jerry@cleanerwindowcleaning.com.
- Do NOT delete the landing page, pop-ups, or game. Every button must stay
  clickable and do something.
- Do NOT break the game progression: Wet → Take Squeegee → Squeegee →
  Reholster → Wipe (extra). Hit Too Hard = -30, window broken.
- Test in a real browser mindset: the game must play on Android Chrome
  with joystick + look drag, and on desktop with WASD + mouse. No
  blocky Lego look — aim for virtually real, immersive first-person
  by default, third-person as a toggle.

## Files

- `index.html` — entire site + game, single file, Three.js via CDN.
- `1000004706_1_5ivd.png` — original mockup, Gallery only.

## When you change the game

1. Fix playability first, then visuals.
2. Keep the 2D fallback working if Three.js fails.
3. Tell the user plainly what you tested and what you could not test.
