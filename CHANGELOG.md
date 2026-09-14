# Changelog

## 0.0.2 (13 September 2026)
- **Modernized Build:** Switched to `esbuild` to reduce the extension size
- **Formatter Fix:** Standard directives (`.data`, `.text`, `.macro`, etc.) inherit the instruction indent instead of snapping to the left
- **Formatter Fix:** Clang-style block alignment for end-of-line comments
- **Formatter Fix:** Fixed an AArch64 bug where relocation modifiers (like `@PAGE` and `@PAGEOFF`) were formatted as comments
- **Formatter Fix:** Added space between closing braces and comments

## 0.0.1 (10 October 2023)
Initial release.