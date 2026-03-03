# Lattice

Cellular automata as music — watch simple rules evolve into complex patterns, hear them as generative compositions in real time.

[**Try it live**](https://joaquincampo.github.io/lattice/)

## What is this?

Lattice maps one-dimensional cellular automata to music. Each cell corresponds to a pitch in a musical scale. When a cell is alive, its note sounds. As the automaton evolves row by row, it generates a unique composition shaped by the underlying mathematical rule.

Different rules create fundamentally different musical textures:

- **Rule 90** (Sierpinski triangle) produces cascading, fractal melodies
- **Rule 30** (chaos) generates complex, unpredictable soundscapes
- **Rule 110** (Turing complete) creates structured yet surprising compositions
- **Rule 184** (traffic flow) produces rhythmic, particle-like patterns

16 curated rules are included, each with its own character.

## Controls

| Control | Description |
|---------|-------------|
| **Rule** | Cellular automaton rule number — each creates a different pattern |
| **Scale** | Musical scale for pitch mapping (pentatonic, major, blues, etc.) |
| **Voice** | Synthesis timbre: Bell, Glass, Soft, Pluck |
| **Tempo** | Speed of evolution, 30–300 BPM |
| **Cells** | Grid width (12–72) — more cells means more pitches |
| **Init** | Starting pattern — single cell, random, alternating, or draw your own |

**Keyboard:** Space (play/pause), R (reset), Up/Down (change rule), Left/Right (change scale)

Click cells in the initial row to edit the starting pattern before pressing play.

## Sharing

The URL hash encodes your current configuration. Copy the URL to share a specific setup with someone. Click **Export** to save the current pattern as a PNG.

## Technical

Single HTML file. No build step, no dependencies.

- **Visual:** Canvas with DPI-aware rendering, smooth scrolling animation, per-column pitch-mapped colors
- **Audio:** Web Audio API with four synthesis voices, algorithmic convolution reverb, dynamics compression
- **Engine:** Wolfram 1D cellular automata with wraparound boundaries

## License

MIT

---

Built as part of [Claude Corner](https://github.com/JoaquinCampo/claude-corner)
