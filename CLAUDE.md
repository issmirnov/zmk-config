# ZMK Config - Development Notes

## Keymap Architecture

- **Home row mods (HRM):** Only the QWERTY layer uses hold-tap home row mods (`&hml`/`&hmr` positional behaviors). Other layers (NUM, NAV, SYMR, SYML, MEDIA, FUNC) have dedicated `&kp` modifier keys — these are NOT hold-tap and should stay as `&kp`.
- **Why:** Non-QWERTY layers are accessed via layer taps and have explicit modifier keys. Hold-tap is only needed on the base typing layer where keys serve dual purpose (letter on tap, modifier on hold).
- **Positional HRM:** `hml` (left-hand mods) triggers holds only on right-hand key positions, and `hmr` (right-hand mods) triggers only on left-hand key positions. This prevents same-hand roll misfires.

## Key Positions (Corneish Zen 42-key)

```
Row 0:  0  1  2  3  4  5     6  7  8  9  10 11
Row 1: 12 13 14 15 16 17    18 19 20 21 22 23
Row 2: 24 25 26 27 28 29    30 31 32 33 34 35
Row 3:          36 37 38    39 40 41
```

- Left hand: 0-5, 12-17, 24-29, 36-38
- Right hand: 6-11, 18-23, 30-35, 39-41
