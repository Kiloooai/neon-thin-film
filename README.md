# Neon Thin Film

Interactive thin-film interference visualizer — watch colors emerge from the interference of light reflected off the front and back surfaces of a film.

Adjust refractive index, maximum thickness, ripple amplitude and speed to see the colors shift and ripple across the gradient. Color modes rotate the hue palette.

## Features

- **Physics‑based rendering**:reflectance computed from equation \(R = 4 r^2 \sin^2(\delta/2)\), \(\delta = 4\pi n d / \lambda\)
- **Three‑wavelength sampling** (red, green, blue) produces realistic interference colors
- **Animated ripple**: traveling sinusoidal thickness variation simulates surface waves
- **Adjustable parameters**:
  - Refractive index *n* (1.00 – 2.50)
  - Max thickness *d* (0 – 2000 nm)
  - Ripple amplitude (nm)
  - Wave speed (ripple propagation)
  - Glow intensity
  - Color mode (hue rotation)
- **Pause / Reset** controls
- **Real‑time** gradient updating

## Physics

For light of wavelength λ incident normally on a thin film of refractive index *n* and thickness *d* (surrounded by air), the path difference between the two reflected waves is \(2 n d\). The phase difference is:

\[
\delta = \frac{2\pi}{\lambda} \cdot 2 n d = \frac{4\pi n d}{\lambda}
\]

The intensity reflectance (fraction of light reflected) is:

\[
R(\lambda) = 4 r^2 \sin^2\!\left(\frac{\delta}{2}\right),
\quad
r = \frac{n-1}{n+1}
\]

For broadband (white) illumination, the perceived color is the combination of \(R(\lambda)\) across the visible spectrum. This simulation samples red (620 nm), green (530 nm), and blue (460 nm) wavelengths, then reconstructs an RGB color.

Adding a traveling ripple to the thickness creates moving interference bands, reminiscent of soap bubble dynamics.

## Usage

Open `index.html` in a browser. Left‑hand controls:

- **Refr. index (n)** – optical density of film (water ≈ 1.33, glass ≈ 1.5, oil ≈ 1.6…)
- **Max thickness (d)** – gradient spans thickness 0 → *d* across the screen
- **Ripple amp** – amplitude of traveling thickness wave (set 0 for static gradient)
- **Wave speed** – how fast the ripple travels
- **Glow** – neon blur intensity (visual only)
- **Color mode** – rotates the hue palette
- **Reset** – restores default parameters
- **Pause** – freeze/resume the ripple animation

The right‑hand stats show current FPS and the numerical values of *n* and *d*.

## Tips

- Higher *n* yields more saturated colors and narrower fringe spacing.
- Increase **Ripple amp** to see dynamic bands flow across the gradient.
- **Color mode** rotates the hue to give different neon looks.
- Set **Ripple amp** to 0 for a static color‑thickness map.

## Live

Hosted on GitHub Pages: https://kiloooai.github.io/neon-thin-film/

## Source

https://github.com/Kiloooai/neon-thin-film
