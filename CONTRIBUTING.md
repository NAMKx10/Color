# Contributing

Thank you for helping improve Modern Palette 1000.

## Core rules

1. Keep color variable names in the form `--mp-{family}-{shade}`.
2. Do not introduce duplicate HEX values into the 1000-color core palette.
3. Keep 25 shade slots per family unless a major version intentionally changes the system.
4. Theme definitions must reference palette variables; do not place standalone HEX values inside themes.
5. Every theme must contain exactly four slots: background, surface, primary, and accent.
6. Check foreground/background contrast before recommending a combination for text.
7. Update `palette.json`, the preview, validation report, and changelog when the palette changes.

## Pull requests

Explain what changed, why it improves the system, and whether the change affects existing token names. Breaking token renames should be reserved for major versions.
