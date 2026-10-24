DeskPort 0.7.4 self-test build for macOS arm64 and NixOS x86_64.

- Choose Settings → Keyboard shortcuts → Change shortcut to record a custom recall combination, save it immediately, or restore the default Meta + apostrophe (Command + apostrophe on macOS).
- Recording temporarily pauses the global binding. Changes update native registration and existing/new viewer workers; occupied bindings report an error. Wayland's desktop-assigned combination remains authoritative.
- Keep the default-on shortcut switch and expand the offline manual to 13 chapters and 67 steps. Recorder and status labels include draft translations in all 22 primary locales.

The macOS app and DMG are Developer ID signed, notarized and stapled. The ZIP is verified after extraction and in the Nix consumer. Linux is built natively from the pinned public source. Activation and physical shortcut/streaming/input acceptance remain manual.

Source: https://github.com/keithxc/deskport/tree/bd28a11d4695d34c348bd9694a3c15f883f8fff2
Core: https://github.com/keithxc/deskport-core/tree/b12d33c8811be6ee96efd45a0aeb14f775903ca1
