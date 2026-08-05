# Omie Aerospace QA

Small hand-curated set of aerospace engineering Q&A pairs. Built as one of the training sources for [Omie](https://github.com/KerbalMissile), a small from-scratch language model.

83 pairs, single-turn. Covers propulsion basics (Isp, delta-v, staging, engine types, nozzles), orbital mechanics (Hohmann transfers, geostationary orbit, escape velocity), aerodynamics (stall, drag, Mach, sonic booms), reentry/materials (Inconel, ablative heat shields), and flight computer / hobby rocketry stuff (apogee detection, static margin, N2O/ethanol, hybrids).

Not scraped, not model-generated. Written by hand because nothing decent already existed for this; everything on HF tagged "aerospace" turned out to be extractive QA over NTSB incident reports (short spans, not real answers) or empty repos. If you know this domain better than the answers here, open a PR, half of this could use tightening.

## Format

```json
{"turns": [{"speaker": "user", "text": "..."}, {"speaker": "omie", "text": "..."}]}
```

One line per example. `speaker` is `user` or `omie`. Swap `omie` for whatever role name your setup expects.

## Why this exists

Wanted a small aerospace source to fold into Omie's training mix alongside general-conversation data (no_robots, oasst1, empathetic_dialogues, personachat). Didn't find a human-written conversational aerospace dataset anywhere, so made one instead of forcing an off-topic fit.

## License

GPL-v3.0
