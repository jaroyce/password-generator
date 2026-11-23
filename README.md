# Squarefrog Password Generator

A single-page password generator. Everything runs in the browser using `crypto.getRandomValues()`; nothing is sent to any server and there are no third-party requests.

Live: https://jaroyce.github.io/password-generator/

## Features

- **Random** passwords: length 8–128, character types, exclude look-alikes, no repeats, and a guarantee of at least one of each ticked type.
- **Memorable** passwords: 3–10 words from the EFF long wordlist, a chosen or custom separator, capitalisation styles, 0–4 numbers as digits or words ("seven"), at the start, end or between words, and an optional symbol.
- **PIN** codes: 4–12 digits.
- Strength meter with bits of entropy and an estimated crack time at 10 billion guesses per second.
- Show/hide, copy, bulk generate with "Copy all", and an optional clipboard clear after 30 seconds.
- Light, dark or automatic theme.
- **Save settings** stores all options (including the theme) in `localStorage` in that browser only. Passwords are never stored.
- Keyboard shortcuts: Space or Enter for a new password, C to copy, H to show/hide.

## Credits

Memorable passwords use the [EFF long wordlist](https://www.eff.org/dice), licensed under [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/us/). Hyphens were removed from three words and `yo-yo` was dropped as a duplicate of `yoyo`, leaving 7,775 words.

## Changelog

### 1.1.0 — 2026-11-23
- New Squarefrog styling (matches Site Crawler), with a header, light/dark/auto theme switcher, and a copyright and version footer.
- New pink key favicon set (SVG, ICO, PNGs, Apple touch icon) and a web app manifest.
- Memorable password mode, including numbers written as words.
- PIN mode.
- Save settings and Reset to defaults.
- At least one of each character type, show/hide, crack-time estimate, clipboard auto-clear, keyboard shortcuts, bulk "Copy all", and accessibility improvements.
- Corrected the strength calculation for "No repeated characters".

### 1.0.3 — 2026-11-23
- Show the version number in the page footer (read from the `version` meta tag).

### 1.0.2 — 2026-11-23
- Removed the Google Fonts dependency; the page now uses system fonts and makes no third-party requests.

### 1.0.1 — 2026-11-23
- Renamed `password-generator.html` to `index.html` for GitHub Pages.

### 1.0.0 — 2026-11-23
- Initial release.
