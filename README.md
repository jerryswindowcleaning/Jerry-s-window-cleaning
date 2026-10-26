# Cleaner Window Cleaning — Website + Window Cleaning Game

Live business site (planned): https://cleanerwindowcleaning.com
Business: Jerry's Window Cleaning, San Diego County
Phone: 217-552-8626 — Email: jerry@cleanerwindowcleaning.com
Rate: $110/hour, regardless of window count. Estimates: 100% free.
Hours: 9am–5pm, 7 days a week. Same-day sometimes possible, never guaranteed.
Service: Inside and out, squeegee / mop / T-bar, ladders. Water-fed pole with
purified deionized water if requested in advance. Talk first about exactly
what the customer expects, only do what they ask.

## What is in this repo

- `index.html` — The whole site in one file: retro landing page, clickable
  magical pop-ups for every button, and the playable window cleaning game
  below the landing page.
- `1000004706_1_5ivd.png` — Original landing design mockup, shown in the
  Gallery section. Upload it alongside `index.html` on hosting.

## How to run it locally

Open `index.html` in Chrome or Safari (not in a chat file viewer — 3D /
WebGL needs a real browser). No build step, no server needed for the basic
page. Three.js is loaded from a CDN, so you need internet for the 3D game.
If Three.js cannot load, the 2D window strip + buttons still play.

## The game — current state (v2, 2026-10-26)

- Walk around a house scene: WASD / arrows on desktop, left virtual
  joystick on phone, drag to look (mouse or touch).
- Camera: first-person by default (through the cleaner's eyes, VR-like),
  V / Camera button switches to third-person (GTA-style, cleaner from behind).
- Walk up to a dirty window until it highlights, or tap a window in 3D or
  in the 2D strip to walk up to it, then clean in order:
  1. Wet Window (Mop / T-Bar) +5
  2. Take Squeegee from Holster +5
  3. Squeegee the Glass +20
  4. Reholster Squeegee +5 — window becomes Clean
  5. Wipe +15 extra
- Hit Too Hard breaks the window: -30 points, that window cannot be cleaned.
- Score, windows cleaned / 5, broken count, current step, and Restart are
  shown in the HUD.
- Discount: "Play & Save: Clean windows in the game and earn a discount on
  your real window cleaning — call 217-552-8626 and mention your score to
  claim it." Discount pop-up at 3 cleaned windows or score 100.
  Do NOT invent a fixed % or $ amount — the discount is confirmed on the
  phone call.

## Known problems to fix next (for Claude Code)

User feedback 2026-10-26: the first version did not play at all on his
phone and looked like Lego blocks. v2 fixed the 2D selection bug, touch
look, joystick, first-person default, and rounded cleaner, but it has NOT
been tested in a live Chrome browser, and it is NOT a true VR-headset
(WebXR) mode. The cleaner is rounded and stylized, not photorealistic,
and textures are procedural, not photographs.

Next work for Claude Code:
1. Test and fix playability in Chrome on Android first, then desktop.
2. Make it look virtually real: realistic house, glass, dirt, lighting,
   shadows, and a realistic cleaner — no blocky Lego look.
3. Keep every button working, keep the discount wording above, keep
   San Diego / $110 / free estimates / 9-5 correct.
4. Keep the site professional and high-resolution, not pixelated.

## For Claude Code — how to use this repo

1. Clone this repo to your computer, or open this folder in Claude Code.
2. In a terminal in this folder, run: `claude`
3. Then prompt, for example:
   "Open index.html and fix the window cleaning game so it is actually
   playable in Chrome on Android and looks realistic, not blocky.
   Keep the landing page, business details, and discount wording exactly
   as they are."
4. Test by opening index.html in Chrome, walking, switching cameras,
   and cleaning all 5 windows. Commit when it plays cleanly.
