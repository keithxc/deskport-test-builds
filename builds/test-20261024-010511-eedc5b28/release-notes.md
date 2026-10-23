DeskPort 0.7.4 self-test build for macOS arm64 and NixOS x86_64.

- Add Settings → Keyboard shortcuts → Global window shortcut, enabled by default and applied immediately.
- Turning the shortcut off releases the system binding and disables the viewer fallback.
- Expand the offline manual to 13 chapters and 66 steps, including background sessions, desktop shortcuts, input/IME/clipboard, picture and sound, browser access and troubleshooting. New manual text includes English and both Chinese scripts.

The macOS app and DMG are Developer ID signed, notarized and stapled. The ZIP passed Gatekeeper after extraction and after Nix installation. Linux was built natively from the pinned public source and passed isolated startup checks. Activation and physical streaming/input acceptance remain manual.

Source: https://github.com/keithxc/deskport/tree/eedc5b2884e80e26d3c94df6bc0a026ab3b1ba01
Core: https://github.com/keithxc/deskport-core/tree/e482f24563b2026693e284fbd8ca54eb420b7896
