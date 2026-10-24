DeskPort 0.7.4 self-test for macOS arm64 and NixOS x86_64.

- Keep the shortcut switch and editable combination on one settings row.
- Temporarily request window-scoped Wayland shortcut inhibition while recording, and offer a mouse/keyboard key chooser when the desktop reserves a combination. Closing or losing focus releases the request. Existing desktop bindings are not silently replaced.
- Support common punctuation, navigation and editing keys, plus F1–F20 on macOS and F1–F24 on Linux. KDE may ask you to resolve a conflict for task-manager combinations such as Meta+1–9.
- Update the offline manual to 13 chapters / 68 steps with chooser text in all 22 primary locales.

The macOS app and DMG are Developer ID signed, notarized and stapled; extracted-ZIP and Nix-consumer Gatekeeper checks passed. Linux is built natively from the pinned public source through the mynix consumer. Package checks are separate from physical keyboard delivery, streaming and input acceptance, which remain pending manual activation.

Source: https://github.com/keithxc/deskport/tree/14a53a913afe06716f67217b604893d9a62cfca8
Core: https://github.com/keithxc/deskport-core/tree/505ae0ccd0a4ead4decb6eaba62585bf278e6dbe
