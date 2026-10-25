# DeskPort window-state self-test

One retained desktop window switches between devices, connection progress and video. Video decoding and rendering run in the GUI process while connection workers retain networking state.

This follow-up preserves fullscreen/maximized state on connect and recall, enables macOS native fullscreen, keeps its controls visible, and fixes a Metal presentation-callback lifetime crash on fullscreen exit.

Windows and macOS packages and native Linux Nix input use source `5eab8059ad7e8e507e977a4bcaf35867a2fad15a`; shared core is unchanged. Native tests cover 16 decoded window-state stages on each desktop platform. Live tests and remaining mouse-resize limitations are detailed in `manifest.json`. Compilation is not a claim of audio, HDR, latency or long-duration acceptance.

macOS packages are Developer ID signed, notarized and stapled. Windows includes Setup and portable packages. Linux is delivered through the fixed public source archive and mynix. Nix activation remains manual.

Corresponding source: https://github.com/keithxc/deskport/tree/5eab8059ad7e8e507e977a4bcaf35867a2fad15a

This is a PC self-test prerelease; it does not replace the stable release. Package license notices are retained. No mobile packages or private device evidence are included.
