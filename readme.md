# Dark AI Sidebar for Zen Browser

Dark theme & seamless styling for the built-in Firefox AI Chatbot sidebar in Zen Browser.

## Why this mod?

Zen Browser disables Firefox's legacy Lightweight Themes in favor of its own native color engine. Because the built-in AI Chatbot sidebar expects a Lightweight Theme to supply its colors, it defaults to light mode (white header and dark text), even when Zen is in dark mode.

This mod bridges the gap:
- Restores full dark mode to the AI Chatbot sidebar (`chat.html`).
- Matches Zen Browser's native dark palette (`#18181b`).
- Automatically adapts when switching between light and dark modes in Zen (`zen.view.window.scheme`).

## Preferences

- **Hide duplicate panel title:** Zen already displays the panel name in `#sidebar-header`. Toggling this on removes the duplicate title inside the chat header to save vertical space.
- **Header background style:** Choose between **Zen Dark** (default `#18181b`), **Pure Black** (`#000000` for OLED displays), or **Midnight Navy** (`#0f172a`).

## How to enable the AI Chatbot in Zen

1. Open `about:config`.
2. Set `browser.ml.chat.enabled` to `true`.
3. Set `browser.ml.chat.sidebar` to `true`.
4. Choose your preferred AI provider in `about:preferences#general` or in the sidebar menu.
