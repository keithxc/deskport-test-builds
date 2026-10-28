Desktop self-test: window movement and display recovery

- The hidden-title-bar setting explains how to move the window directly below its switch.
- On macOS, hold Control+Command and drag the remote picture to move the local window; remote input is released during the gesture.
- Display preparation retries transient legacy host refusals with a bounded, cancellable delay and records clearer host rejection diagnostics.
- Native Wayland keeps decorations stable across Devices/remote-view transitions and preserves the session during explicit decoration changes.

macOS arm64 ZIP and DMG are signed, notarized and verified. Windows x64 full Setup and portable ZIP passed package, PE and payload-consistency audits; their GitHub SHA-256 digests and sizes match.

Linux delivery is pending a native compositor fix: changing the hidden-title-bar setting while fullscreen can restore an incorrect normal-window size. The affected path is native Wayland; the macOS and Windows window paths are separate. Published installers and their recorded source remain unchanged. Physical streaming/input acceptance remains manual.

Source: https://github.com/keithxc/deskport/tree/39ee3a1b379deef465e2aa97e00bde35b1a89584
Core: https://github.com/keithxc/deskport-core/tree/27caf8317b959da9c240dd5f8843b319d7fa74b7
