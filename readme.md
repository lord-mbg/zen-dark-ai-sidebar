# Dark AI Sidebar for Zen Browser

CSS-only Zen Mod for the built-in Firefox AI Chatbot sidebar. Its default mode reveals the **actual active Workspace background** behind the AI controls; it does not copy or hard-code workspace colors.

## Why this mod?

Zen paints each Workspace's colors behind the browser UI, but Firefox's AI sidebar and its embedded document have opaque backgrounds. This mod makes only the AI sidebar and the AI page's own canvas/header transparent, so Zen's existing background shows through. The chatbot provider's website remains independent.

Switching Workspaces updates the background without changing the mod. Non-AI sidebars are untouched. The solid-color options remain available if transparency does not work with a particular platform or theme.

## Preferences

- **Hide duplicate panel title:** Hides the internal panel switcher when Zen already displays the panel title. This only affects layouts where Firefox displays that switcher.
- **Header background style:** **Match Workspace Theme** (default), **Solid Zen Dark**, **Pure Black (OLED)**, or **Midnight Navy**.

Text contrast inside the AI page follows Zen's `zen.view.window.scheme` preference (dark, light, or system). CSS-only mods cannot read the Workspace's derived text color across the embedded-document boundary; on a custom light Workspace with the system set to dark, choose light mode or a solid header if controls are hard to read.

## How to enable the AI Chatbot in Zen

1. Open `about:config`.
2. Set `browser.ml.chat.enabled` to `true`.
3. Set `browser.ml.chat.sidebar` to `true`.
4. Choose your preferred AI provider in `about:preferences#general` or in the sidebar menu.
