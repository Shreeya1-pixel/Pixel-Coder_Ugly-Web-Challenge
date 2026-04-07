# Pixel Coder · Ugly Web Challenge
LIVE AT - https://shreeya1-pixel.github.io/Pixel-Coder_Ugly-Web-Challenge/

**NoMind™ AI — Insight Failure.** A single-file satire of a fake productivity startup: loud, hostile, and deliberately unusable. Built for the Ugly Web Challenge.

---

## What you’re signing up for

The page looks like a product landing page for about **three seconds**. Then the “chaos layer” activates. Everything below is intentional. There is **no mute button**. There is **no off switch**. That is the point.

---

## Feature inventory

### Audio — Web Audio glitch engine

Synthesized in the browser (no external sound files). Randomized **waveforms** (sawtooth, square, triangle) with random pitch and gain for short digital glitches.

- **Fire-brigade / siren** — square-wave sweep (rough emergency-vehicle energy).
- **Low “honk”** — sawtooth drop (comic relief, still obnoxious).
- **Ambient chaos** — timers fire often; each trigger may or may not play a sound (`Math.random()`).
- **Click** — every click can trigger the glitch player (first interaction may require a gesture for audio context on some browsers).
- **Scroll** — rare glitch on scroll.

Volume and texture vary per hit. **No user controls.** Corporate confidence.

---

### Brain Rot Chat (chatbot disruption)

- Type in the **Brain Rot Chat** field: each character renders in a **random ugly font stack** (Courier, Times, Comic Sans, Impact) with clashing colors.
- **Hard limit: 3 characters.** On the 4th keystroke:
  - Full-viewport **MESSAGE TOO LONG!!!! STOP!!!!** overlay (centered, shaking).
  - Input **locks** briefly, then **clears** after ~2.5s so the cycle can repeat.
  - **Popup spam** — multiple yellow warning boxes in quick succession.

---

### Yellow warning popups

- Spawn on an interval and stack over the viewport.
- **Misleading CTA:** **Reduce Popups** removes the current box and **spawns three more**.
- **Close (X)** is unreliable: sometimes closes, sometimes **duplicates** popups.
- Copy mixes **fake compliance** (“cookies,” “CPU smiling”) with **passive-aggressive** lines:
  - *Why are you still here?*
  - *This is not helping you.*
  - *Stop clicking things.*
  - *You could have left.*

---

### Scrolling — infinite page trap (polite edition)

- When you **stay** within ~140px of the **document bottom** for **2–3 seconds** (randomized dwell), the page **scrolls back to top** (smooth or instant, random).
- Scroll away before the timer finishes → **timer cancels**; you keep control until you commit to the bottom again.
- Sometimes an **`alert()`** fires with lines like *You are not done yet.* / *Scrolling is temporary.*

Extra bottom padding keeps **Contact Us** readable above the fixed nav before the trap fires.

---

### EXIT button — scale mayhem

- The **EXIT** CTA uses a **1 second** CSS transition on hover: **`hover:scale-[10]`** — the button can blow up to absurd size, making the joke visually and physically dominant.

---

### Buttons that fight back (`annoying-btn`)

- **Start Now**, **Optimize Life**, **EXIT**, and bento tiles: on hover, random **translate + rotate** nudges.
- Occasional **jump-away** keyframe burst — still clickable in theory, frustrating in practice.
- **FREE PRODUCTIVITY** still **teleports** inside its hero box on hover (`moving-target`).

---

### Full-screen loading freeze

- Random full-viewport overlay: *Processing…*, *Optimizing your experience…*, and similar corporate lies.
- Blocks interaction for **~2–5 seconds**, then disappears — sometimes **chains** a second freeze shortly after.

---

### Cursor chaos

- After chaos engages: **system cursor hidden**, **fake neon ring** follows the pointer.
- Ring **scales up and down over a 10s cycle** (CSS keyframes, infinite alternate).
- Border color **randomizes every ~2s** for extra visual noise.

---

### Other hostility

- **Start Now** opens a **system overload** modal (48-hour queue fiction).
- **Optimize Life** jumps scroll to a **random** vertical position.
- **Blockade** / **popups** / **alerts** / **freezes** stack for layered frustration.

---

## Run locally

If you want a local server: `python3 -m http.server 8000` in this folder, then open [http://localhost:8000](http://localhost:8000). You can also open `index.html` in a browser directly.

---

## Stack

- Single **`index.html`** — Tailwind CDN, Google Fonts, Material Symbols, inline CSS + JS.
- **Web Audio API** for synthesized SFX.

---

## Disclaimer

Satire. Loud. Do not subject unwilling participants without warning.

---

**NoMind™** — *We don’t solve problems. We create them.*
