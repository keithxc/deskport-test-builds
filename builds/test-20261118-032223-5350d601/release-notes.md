PC self-test build for macOS arm64 and NixOS x86_64. Application version remains 0.7.8.

Includes the consolidated desktop session, display, input, streaming policy and lifecycle work. Experimental Seamless development remains separately gated.

The macOS ZIP is Developer ID signed, notarized and stapled. Linux uses the pinned source archive through Nix. Package builds and isolated regression checks passed; live streaming and input acceptance follow manual activation.

Source: [5350d601](https://github.com/keithxc/deskport/commit/5350d6017904b40cb12404ac20e7645e88169350). Core: [44f2289](https://github.com/keithxc/deskport-core/commit/44f228995f23435d2aa93b661d2f105d3664b338). See manifest.json for immutable input and asset hashes.

Final fixture validation: [c02faf05](https://github.com/keithxc/deskport/commit/c02faf057d3a3fdd0b1b568ebbf122ba52086cb7). Only test fixtures differ from the packaged source; production and packaging inputs are identical.
