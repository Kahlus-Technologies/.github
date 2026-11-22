# Draft notes for the org profile (delete before the PR)

This file holds the claims table and the proposals for firstmate. It is not part of the page. The wording in `README.md` is a content draft. The visual design waits for the Kahlus design language.

## Claims and sources

All repo paths are in Kahlus-Technologies public repos at the commit seen on 2026-11-22.

| Claim on the page | Source |
| --- | --- |
| Research in robotic cold plasma and closed-loop neurotechnology | kahlus.com title "Robotic cold-plasma research" and home text "Kahlus also works on EEG forecasting and assistive-mobility controls"; Kahlus-V2 README (closed-loop sleep stimulation) |
| We publish methods, code and results that went against us | Kahlus-V2 README ("Losses are results. Nulls and negative results are reported."); Kahlus-V1 README ("Report the loss") |
| K7: 5,768 SHHS-1 nights, relative risk 5.01 [4.83, 5.18] | Kahlus-V2 `results/k7-shhs1/2026-11-21-dda45d8/summary.md` |
| K7: 2,031 sealed MESA nights, 3.79, scored once | Kahlus-V2 `results/k7-mesa/2026-11-21-3a895b0/summary.md` and `docs/results/mesa_final_looks/run_k7.json` |
| Time-shifted fake trigger about 1.0 (0.995 and 1.004) | same two summaries, rotated-trigger gate |
| "No sound was played", replay measures timing only | Kahlus-V2 README Results section and both summaries |
| A click before an arousal can wake the sleeper; stimulation can deepen slow-wave sleep | Kahlus-V2 README "What this is" |
| Release v0.2-k7 exists | `gh api repos/Kahlus-Technologies/Kahlus-V2/releases/tags/v0.2-k7` (published, not draft) |
| Preregistration file and SHA-256 recorded in every result file | Kahlus-V2 `docs/prereg/k1-k7.md` rules 2 and 7 |
| MESA seal enforced by a guard in code | Kahlus-V2 README "Sealed test cohort" and `docs/results/mesa_exposure.md` |
| Features end at prediction time; shift control | Kahlus-V2 README "Causal everything", "Shift controls" |
| V1: r = 0.972 came from overlapping windows and was retracted | Kahlus-V1 README "The headline result"; `docs/paper/iecbes2026/claims_audit.md` (126 of 127 samples shared) |
| V1: recurrent model did not beat a ridge baseline on strictly future samples | Kahlus-V1 README table ("lose to persistence / ridge"); IECBES draft abstract |
| V1: split manifest frozen before preprocessing | Kahlus-V1 README "Why this exists" |
| Plasma arm: six axes, path following, logs each move | kahlus.com home and /plasma |
| Position error under 0.1 mm across 50 commanded bench points | kahlus.com home ("<0.1 mm position error across 50 commanded bench points") and /plasma roadmap ("A 50-point position test is complete") |
| 40 °C thermal cutoff, hardware e-stop outside the software | kahlus.com /plasma "Thermal cutoff and e-stop" |
| Arm is PAROL6 by Source Robotics; Kahlus built board, sensing, planning, software | kahlus.com /plasma "What Kahlus made" |
| No treatment effect evaluated; not cleared for clinical use | kahlus.com /plasma "Use and evidence" |
| IECBES 2026: accepted, 9 to 11 Dec 2026, Kuala Lumpur, authors Patel, Zaidi, Garg | kahlus.com /research item 2; Kahlus-V1 `docs/paper/iecbes2026/` |
| IMECE 2026: accepted, abstract only, Vancouver | kahlus.com /research item 5 |
| ISEC 2026: presented 14 Mar 2026, Princeton, extended abstract and poster, sole author | kahlus.com /research item 10 |
| "Nothing is called published until it is in a proceedings index" | kahlus.com /research footer note |
| kahlus-bench, neuroforecast, kahlus-research, kahlus-skills, Subvox, Sotto, mentra-eeg-miniapp, hil-failure-modes descriptions | each repo's own README and GitHub description |
| mentra-eeg-miniapp signal is synthetic | its README "Status" section |
| hil-failure-modes bench runs not done yet | its README "Test status" |

## Needs a captain decision

1. **IECBES is accepted, not published.** The brief said "published". kahlus.com says accepted, to be presented 9 to 11 Dec 2026, and says nothing is "published" until it is in a proceedings index. The draft says "accepted". Public repo files do not state a publication either.
2. **Paper title.** The site title is "Leakage-Controlled Evaluation of EEG Future-Window Forecasting in Held-Out Subjects". The Kahlus-V1 draft file (V7.2) has an older title ("Developing an Evidence-Gated Framework for Leakage-Controlled EEG Forecasting"). The draft uses the site title.
3. **Homing-Rocketry is left out.** Its README title is "MANPADS Rocket & Launcher Prototype". It does not fit a research-lab page. Say if you want it listed anyway.
4. **Also left out:** sotto-empty (the repo is empty) and subvox-dictate (a fork of the Hex dictation app).
5. **"Non-commercial" is not on the page.** kahlus.com shows a price target ($6,000 to $8,000) and a "Work with us" page, so the draft does not say non-commercial.
6. **The K7 figure lives on the unmerged branch `fm/kahlus-figures` of Kahlus-V2.** The PNGs in `profile/assets/` are copies. The figure text is small on a phone. A regenerated, narrower version is possible with `scripts/figures/make_figures.py` on that branch.
7. **Links in kahlus-bench and kahlus-skills READMEs point to `ptlnextdoor/...`.** The page links to the `Kahlus-Technologies` copies.

## Proposed org settings (not applied)

- **Description:** Robotic cold-plasma and closed-loop neurotechnology research. Preregistered tests, sealed held-out data, and results published as they come, including the ones that went against us.
- **Website:** https://kahlus.com
- **Location:** not stated on kahlus.com. The plasma lab is at San Jose State University, so "San Jose, California" is a candidate. Needs the captain's answer.

## Proposed pinned repositories (web UI, 6)

1. Kahlus-V2 (arousal timing, K7 result)
2. Kahlus-V1 (leakage-controlled EEG forecasting, IECBES 2026)
3. kahlus-bench (sealed benchmark)
4. neuroforecast (directed-information graphs)
5. kahlus-skills (agent skills)
6. kahlus-research (Replay Lab)

## Brand assets found

- Wordmark: Kahlus-V2 `docs/assets/kahlus-wordmark-{light,dark,source}.png`. The draft banner traces `kahlus-wordmark-source.png` into SVG paths.
- Monogram "K" vector: https://kahlus.com/icon.svg
- Site look: black and white, JetBrains Mono and Instrument Sans, one muted pink accent (#eca8d6) on a small square marker. Off-white #ecebe7 and near-black #020204 appear in the site CSS.
