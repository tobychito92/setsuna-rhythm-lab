# SETSUNA · Rhythm Lab v0.6

[Play on GitHub Pages](https://tobychito92.github.io/setsuna-rhythm-lab/)

Three full songs, native portrait/landscape, NORMAL 06 / HARD 12 / EXTREME 16, audio calibration and autoplay. v0.6 rebuilds all nine charts from layered stereo audio analysis. Notes arrive at the judgement line at their measured attack times; approach speed only changes travel time.

| Song | NORMAL | HARD | EXTREME |
|---|---:|---:|---:|
| Setsuna Hanabi | 384 | 936 | 1158 |
| Upside Down Kiss | 236 | 622 | 795 |
| Dance With You | 286 | 625 | 851 |

Chart analysis separates harmonic/percussive estimates, emphasizes center harmonic energy for lead/voice candidates, and detects backing onsets separately. Lead pitch estimates influence lane movement; sustained harmonic energy determines hold ends. Doubles require simultaneous events from distinct layers. Every head stores an evidence event ID. The BPM estimate is diagnostic only: note times are measured attacks, not repeated timer/grid ticks. NORMAL selects prominent attacks; HARD/EXTREME retain additional details with two-hand scheduling.

This is signal-based transcription, not isolated vocal stems, lyric/phoneme recognition or hand-authored Rhythm Hive charts. Lead instruments can enter the voice estimate. Real-song musical transcription quality and physical iPhone latency need listening/touch review. No claim of perfect synchronization or original-game equivalence is made.

Best scores are separated by chart revision; previous records remain in local storage. `npm test` runs 52 Node tests. `python3 -m unittest discover -s tests -p 'test_musical_analysis.py'` runs two synthetic-audio tests. `python3 scripts/musical_chart.py` reanalyzes audio; `--from-analysis` rebuilds charts from saved evidence. `python3 scripts/build-offline.py /absolute/output.html` creates the self-contained version.

Source dependencies: Python, NumPy, SciPy, Pillow (import utility), FFmpeg, and Node. `dist/` is the modular web build. `index.html` on GitHub is a standalone compiled artifact; `Setsuna_Rhythm_Source.zip` contains source, audio and analysis.

Music/artwork belong to their respective rights holders; no third-party asset license is granted here.
