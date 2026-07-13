# Dactyl Manuform 5x6 ZMK Config

## Flashing (nice!nano split)

1. Build via GitHub Actions and download the `firmware` zip artifact.
2. Unzip it and locate the two UF2 files (left and right).
3. Flash left side:
   - Plug in the left nice!nano over USB-C.
   - Double-tap reset (NICENANO drive appears).
   - Copy the left UF2 to NICENANO.
   - Wait for auto-eject/reboot, then unplug.
4. Flash right side:
   - Plug in the right nice!nano.
   - Double-tap reset.
   - Copy the right UF2 to NICENANO.
   - Wait for auto-eject/reboot.

## Update rules

- Keymap-only changes: flash left side only (central side).
- ZMK version, split transport, or matrix/hardware changes: flash both sides.

## Troubleshooting

- If NICENANO does not appear: try a data-capable USB cable and double-tap reset faster.
- If halves do not connect after flashing: reflash both sides from the same build output.
