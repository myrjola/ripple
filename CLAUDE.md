# Ripple - Meditation Timer

Simple meditation timer built with vanilla HTML, CSS, and JavaScript.

## Tech Stack
- HTML, CSS, JavaScript (no frameworks) in index.html and style.css
- PWA with service worker in manifest.json and sw.js

## Guidelines
- The look is the Still Water design: a WebGL lake behind a ring dial. New UI keeps its palette and type.
- `MeditationTimer` owns timing, bells, wake lock and media session and never touches the DOM; the view renders from its events.
- Nothing renders while the page is hidden, so timing must never depend on the frame loop.
