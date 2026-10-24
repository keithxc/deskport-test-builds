Private-use desktop test build for Linux x86_64, macOS arm64 and Windows x64.

The application keeps one main window for Devices, connection progress and the selected desktop. Encoded video is decoded and presented in the main process using the existing native GPU renderers. Network sessions retain isolated worker state.

Includes focus-release boundaries, local text composition, physical key mapping, relative pointer capture, connection confirmation, and canvas lifetime fixes. Native isolated renderer tests exercise resize, session switching, live hide/minimize/recall and teardown. These tests do not establish live-host streaming, physical input, HDR, audio or latency acceptance.

Source: https://github.com/keithxc/deskport/commit/1cb38bb0eb881ad54d7e694eaa40e21fec2d1ef2
Shared core: https://github.com/keithxc/deskport-core/commit/505ae0ccd0a4ead4decb6eaba62585bf278e6dbe

Exact package hashes and verification scope are recorded in manifest.json and the platform checksum files. Upstream notices remain inside the packages. No mobile artifacts or separate source/relink archives are uploaded. Activation remains manual.
