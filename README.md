# Neon Thin Film

Interactive thin-film interference simulator — watch colors dance across a gradient of thickness, with optional traveling ripples and neon glow.

Thin films (soap bubbles, oil slicks, anti-reflective coatings) create colors by interference: light reflecting off the top and bottom surfaces combines with a phase shift, producing constructive/destructive patterns that vary with thickness. This simulation computes normal-incidence reflectance for red, green, and blue wavelengths and maps them to a full-width canvas gradient.

Canvas glow, clean controls, and a ripple mode for animated wave motion.

## Controls

- **Refr. index (n)** — film refractive index (1.00 – 2.50). Higher n increases fringe spacing and contrast.
- **Max thickness (d)** — maximum film thickness in nanometers (0 – 2000). Thickness sweeps left → right.
- **Ripple amp** — amplitude of a traveling sine-wave thickness modulation. Creates a waving interference pattern.
- **Wave speed** — how fast the ripple travels across the film.
- **Glow** — neon bloom intensity (drop-shadow filter strength).
- **Color mode** — four modes:
  - 0: Direct RGB from interference
  - 1: Hue-rotated (+180°)
  - 2: CMY-inspired remapping
  - 3: Psychedelic saturation boost + hue shift

Buttons: **Reset** (restore defaults) | **Pause/Resume** (freeze time & ripple)

---

Built with vanilla HTML/CSS/JS — no libraries.

Live demo: https://kiloooai.github.io/neon-thin-film/
