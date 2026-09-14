# Changelog

## 0.0.3 (13 September 2026)
- **Formatter:** Fixed a bug where user setting for `arm.formatting.labelsCase` (`upper` or `lower`) was being ignored
- **Settings:** Added an `off` option to `arm.formatting.labelsCase` and made it the default behavior

## 0.0.2 (13 September 2026)
- **Modernized Build:** Switched to `esbuild` to reduce the extension size
- **Formatter:** Standard directives (`.data`, `.text`, `.macro`, etc.) inherit the instruction indent instead of snapping to the left
- **Formatter:** Clang-style block alignment for end-of-line comments
- **Formatter:** Fixed an AArch64 bug where relocation modifiers (like `@PAGE` and `@PAGEOFF`) were formatted as comments
- **Formatter:** Added space between closing braces and comments

## 0.0.1 (10 October 2023)
Initial release.