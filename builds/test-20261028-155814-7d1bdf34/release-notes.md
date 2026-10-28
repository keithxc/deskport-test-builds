With the remote canvas title bar hidden, hold **Control+Command** and drag inside the picture to move the window, or drag an edge or corner to resize it. The setting and information panel explain both gestures. Ordinary pointer gestures remain available to the remote canvas. Devices and the visible system title bar retain native controls.

Local gestures suspend remote input. Modifier release and window transitions cancel geometry changes safely. Fullscreen return restores the original frame, including rapid re-entry.

Validation: 47 native macOS cases with actual NSWindow geometry and process-local events; 31 UI cases; 6 canvas input cases; 8 preferences cases; 18,476 packaged translations; shared-core checks. The added fullscreen regression fails on the previous implementation and passes here. Developer ID signatures, Apple app/DMG notarization, stapled tickets, extracted-ZIP Gatekeeper and isolated bundled-host loader checks passed.

These isolated checks do not establish physical dragging, mixed-DPI behavior or connected remote streaming/input acceptance. Activation and live testing remain manual.

This macOS self-test uses [DeskPort `7d1bdf34`](https://github.com/keithxc/deskport/tree/7d1bdf3477b4227b3e5a002ed7941b4f6a93a2d4) and [core `866c0954`](https://github.com/keithxc/deskport-core/tree/866c09547cd47d4b26a0725374e70614cf2845db). Existing [Linux delivery](https://github.com/keithxc/deskport-test-builds/releases/tag/test-20261028-203847-a45eb92f) and [Windows installers / previous macOS rollback](https://github.com/keithxc/deskport-test-builds/releases/tag/test-20261028-185000-39ee3a1b) retain their original identities.

Installers, checksums and small provenance records only. Exact source commits are linked above; package notices are preserved. This is a self-test prerelease.
