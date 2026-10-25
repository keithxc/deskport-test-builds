Desktop self-test: persistent single window with in-process video decoding and presentation.

Fixes authenticated video startup, zero-size canvas replacement and recovery when a key-frame request is lost while a retained session is paused. Native ten-stage canvas tests pass on Windows, macOS and Linux. Live video was checked in all six platform directions, including takeover, Devices-to-desktop recall and simulated mouse clicks. Cycle rejection was also verified. Tests used LAN IPv4; hostname paths encountered display-negotiation timeouts. Audio, HDR, latency and long-duration reliability are not accepted by this run.

macOS packages are Developer ID signed, notarized and stapled; extracted ZIP Gatekeeper verification passed. Windows includes Setup and portable packages. Linux is delivered through the pinned source archive and native Nix build. Complete macOS and NixOS consumer configurations were prebuilt; Nix activation remains manual.

Source: https://github.com/keithxc/deskport/tree/3f1f44cbc7635ae1bda6264f455f28dae3ddc667
Core: https://github.com/keithxc/deskport-core/tree/505ae0ccd0a4ead4decb6eaba62585bf278e6dbe
mynix pin: 576b9fdc945c13da5d064b3d26184e90da01e9d3

This is a PC self-test prerelease. Existing releases and rollback packages are retained. No mobile artifacts are included. See manifest.json and SHA256SUMS.txt for exact source and asset identities.
