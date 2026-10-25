# DeskPort immediate desktop recall self-test

Returning from Devices now reuses the existing canvas, decoder and ready frame. It no longer shows a fresh connection animation while waiting for a new key frame. macOS also preserves the native outer-window size when restoring its Devices toolbar, preventing an unnecessary remote resolution change.

All three final packaged consumers passed 16 native presentation stages, including recall with new frames withheld, fullscreen, maximize and resize. QML: 31 passed; session manager: 10 passed. Live mouse return was checked on macOS, Windows and Linux; decoder and remote-mode counters did not increase. Windows used the tray menu to open Devices; macOS and Linux used native close and application activation. These checks do not accept audio, HDR, latency or long-duration behavior.

macOS packages are Developer ID signed, notarized and stapled. Extracted ZIP and final Nix consumer passed Gatekeeper. Both complete Nix configurations were built; activation remains manual.

Source: https://github.com/keithxc/deskport/tree/8b20ede75791666055863f1c74e74d5695d14cf2
Shared core: `505ae0ccd0a4ead4decb6eaba62585bf278e6dbe`

PC test packages only; notices preserved. No separate source/relink archives or mobile assets. Exact hashes and validation scope are in `manifest.json` and `SHA256SUMS.txt`.
