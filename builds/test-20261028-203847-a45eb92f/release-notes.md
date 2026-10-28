Desktop self-test: native Wayland window restore

The hidden-title-bar toggle now preserves the normal client size when leaving fullscreen or maximized state under native Wayland. Expanded windows keep their native surface and input focus, while normal-window decoration refresh retains the existing input-release behavior. The setting includes platform-specific window movement help.

The pinned Linux Nix consumer package and complete system configuration built successfully. Isolated CLI/sidecar smoke passed. Native KWin checks passed 92 geometry stages, 13 focused state cases, 3 worker IPC cases and 10 window-frame cases. Core, translation, binding, host, UI, session and canvas regressions passed. Offscreen window tests passed 6 cases, with 4 native-only cases explicitly skipped and covered by the native suite.

This release records the Linux Nix delivery. macOS and Windows installers remain at their separately verified source revision in the [companion release](https://github.com/keithxc/deskport-test-builds/releases/tag/test-20261028-185000-39ee3a1b). The macOS package remains signed and notarized. The Windows Setup was installed and its 676 payload hashes and resident service health verified. No installers were relabelled or replaced.

Both Nix consumer configurations are prepared for manual activation. Physical streaming, input, drag ergonomics and latency acceptance remain manual. The isolated native fixture checks acknowledged Qt state and does not assert compositor-side minimization.

Source: https://github.com/keithxc/deskport/tree/a45eb92fd449216d6968241843885adf9160ffbb
Core: https://github.com/keithxc/deskport-core/tree/27caf8317b959da9c240dd5f8843b319d7fa74b7
Consumer configuration: https://github.com/keithxc/mynix/commit/2318856b17a197d8ff09212f4202d0b71a5d2ff5

Only provenance and checksums are uploaded here. Nix obtains the exact public source archive referenced in the manifest; no additional source or relink archives are uploaded.
