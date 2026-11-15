# SETSUNA · Rhythm Lab v0.7

[Play on GitHub Pages](https://tobychito92.github.io/setsuna-rhythm-lab/)

Three full songs, NORMAL / HARD / EXTREME, portrait and landscape layouts. v0.7 adds diagonal, curved, return and golden trace slides, along with original synthesized tap, trace, flick and tail sounds. Hit sounds have independent volume and a preview button. Chart revisions keep previous best scores separate.

The web release consists of `index.html` and `rhythm-v07.mjs`. Its loader reuses existing embedded song and cover data from the immutable v0.6 commit; this update adds no music or artwork files. Initial loading requires network access. The standalone offline HTML is maintained separately. The source ZIPs retained in this repository are earlier v0.6/v0.4 archives and do not represent v0.7.

Validation on the recovered v0.7 modules: 52 Node tests and two synthetic audio analysis tests pass. Tests include complete runs of all nine charts, 30/60 FPS timing simulations, two-hand scheduling, input geometry, score isolation and onset evidence. Gesture path anchors are checked against analyzed audio events with the same 25 ms tolerance as note heads.

This is signal-based transcription, not isolated vocal stems or hand-authored Rhythm Hive charts. Automated tests do not establish musical transcription accuracy or physical iPhone input latency. Music/artwork belong to their respective rights holders; no third-party asset license is granted here.
