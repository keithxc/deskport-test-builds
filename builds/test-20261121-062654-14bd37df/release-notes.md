# DeskPort 2.9.0 PC Self-Test (`test-20261121-062654-14bd37df`)

Temporary PC self-test build for Batch 1 mouse latency optimizations.

## Source Provenance

- Source repository: `https://github.com/keithxc/deskport`
- Source revision: `14bd37df3c7876dc4654a9c4ca6058b731f17b14` (`codex/mouse-latency-batch1`)
- Core revision: `49c13048b9e91b8638335a87d20cf9c545039b6d`
- Source archive NAR hash: `sha256-tMLx7HcnLVl+wFgXIeiINQ/XEmEaHdw9vCfKdezhf7k=`

## Summary of Changes

- Eliminate embedded-canvas IPC wakeup stall (`CanvasBridge` SDL wakeup event, motion coalescing, direct IPC socket waiting on `!m_ThreadedExec`, skipping redundant `canvas-state` IPC on hovered pointer motion, and flushing `QLocalSocket` on `MultiSessions::canvasInput`).
- Remove Sunshine's 10 ms delayed `BUTTON_LEFT` release hack in absolute mouse mode (`host/overlays/patch-host-mouse-latency.py`).
- Lower `InputActivity` motion wake threshold from 6 px to 3 px with immediate 60 fps burst ceiling (`host/common/inputactivity.h`).

## Verification

- macOS arm64: Developer ID signed, app + DMG notarized and stapled, extracted ZIP passed Gatekeeper and isolated bundled Sunshine loader check.
- Windows x64: Setup EXE + portable ZIP passed PE version (`2.9.0`), payload parity, and package audit checks.
- Activation and live streaming/mouse-latency acceptance remain manual.
