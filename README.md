# Path B shell

Builds an unsigned iOS app shell: Unity 6000.3.10 player (IL2CPP) with the [HybridCLR](https://github.com/focus-creative-games/hybridclr)
interpreter (MIT) and a small boot stub. The shell contains **no game code and no game assets**; a separate Windows tool adds
the player's own game files to it and produces the final IPA.

This repo only holds the build workflow. The Unity Xcode export it builds is kept private because it contains Unity's own
files; only the finished app is published, as `PathB-shell-unsigned.ipa` on the Releases page.
`export.txt` pins the export commit that the next build uses.