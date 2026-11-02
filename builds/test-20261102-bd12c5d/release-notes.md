# Data saver text recovery test

Fix blurry text after window switches by preserving sparse native encoder time and protecting a fresh picture's first quality attempt. Refinement, retries and requested keyframes remain deliverable; the average bitrate target is unchanged.

Two 42-second native HEVC replays passed 14/14 and 15/15 sustained text checks at 2040x1228, with at most 20 ms host-encoder recovery and about 226–227 MB/hour estimated IPv4 video traffic including FEC. The low-budget negative control still fails text acceptance rather than silently lowering the criterion. These are local encoder results; network, capture and client presentation need installed live acceptance.

Targets: signed/notarized macOS arm64 package and native NixOS x86_64 source build. Activation remains manual. Exact desktop/core commits and asset hashes are in manifest.json; no separate source or relink archives are uploaded.
