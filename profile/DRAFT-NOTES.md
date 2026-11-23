# Draft notes for the org profile (delete before the PR)

This file holds the claims table and the proposals for firstmate. It is not part of the page. The wording in `README.md` is a content draft. The visual design waits for the Kahlus design language.

Scope rule: only public repos appear. Kahlus-V2, neuroforecast, kahlus-bench and kahlus-research became private on 2026-11-23 and are removed from the page, the pins and this table. Public repos on 2026-11-23: Kahlus-V1, kahlus-skills, subvox, sotto, subvox-dictate, hil-failure-modes, mentra-eeg-miniapp, Homing-Rocketry, sotto-empty, .github.

## Claims and sources

| Claim on the page | Source |
| --- | --- |
| Research in robotic cold plasma and EEG forecasting | kahlus.com title "Robotic cold-plasma research" and home text "Kahlus also works on EEG forecasting and assistive-mobility controls" |
| We publish methods, code and results that went against us | Kahlus-V1 README ("Report the loss", "Publishing the reconstruction loss and the isolated-forecast loss is the point") |
| V1: r = 0.972 came from overlapping windows and was retracted | Kahlus-V1 README "The headline result"; `docs/paper/iecbes2026/claims_audit.md` (126 of 127 samples shared) |
| V1: recurrent model did not beat a ridge baseline on strictly future samples | Kahlus-V1 README table ("lose to persistence / ridge"); IECBES draft abstract |
| V1: remaining claim is the evaluation protocol, not forecasting skill | Kahlus-V1 README "Honest scope"; IECBES draft abstract |
| Split rules fixed before preprocessing; held-out subjects, sites, datasets | Kahlus-V1 README "Why this exists" and "The tasks" |
| Leakage audits: record reuse, held-out overlap, repeated windows, forbidden target metadata | Kahlus-V1 README "Current Scaffold" |
| Models scored against simple baselines; competitor registry | Kahlus-V1 README "Why this exists", "Current Scaffold" |
| Plasma arm: six axes, path following, logs each move | kahlus.com home and /plasma |
| Position error under 0.1 mm across 50 commanded bench points | kahlus.com home and /plasma roadmap ("A 50-point position test is complete") |
| 40 °C thermal cutoff, hardware e-stop outside the software | kahlus.com /plasma "Thermal cutoff and e-stop" |
| Arm is PAROL6 by Source Robotics; Kahlus built board, sensing, planning, software | kahlus.com /plasma "What Kahlus made" |
| No treatment effect evaluated; not cleared for clinical use | kahlus.com /plasma "Use and evidence" |
| IECBES 2026: published (captain standing instruction, 2026-11-18: accepted 18 Sep, final manuscript submitted), presented 9 to 11 Dec 2026, Kuala Lumpur, authors Patel, Zaidi, Garg | captain instruction; kahlus.com /research item 2 (lists it as accepted); Kahlus-V1 `docs/paper/iecbes2026/` |
| IMECE 2026: accepted, abstract only, Vancouver | kahlus.com /research item 5 |
| ISEC 2026: presented 14 Mar 2026, Princeton, extended abstract and poster, sole author | kahlus.com /research item 10 |
| kahlus-skills, Subvox, Sotto, mentra-eeg-miniapp, hil-failure-modes descriptions | each repo's README and GitHub description |
| mentra-eeg-miniapp signal is synthetic | its README "Status" section |
| hil-failure-modes bench runs not done yet | its README "Test status" |

## Open points

1. **IECBES is written as "published"** per the captain's standing instruction. kahlus.com still lists it as "Accepted" and says nothing is "published" until it is in a proceedings index. The site and the page disagree until the site is updated.
2. **Paper title.** The site title is "Leakage-Controlled Evaluation of EEG Future-Window Forecasting in Held-Out Subjects". The Kahlus-V1 draft file (V7.2) has an older title. The draft uses the site title.
3. **Homing-Rocketry is left out** (captain confirmed). Also left out: sotto-empty (empty repo) and subvox-dictate (a fork of the Hex dictation app).
4. **"Non-commercial" is not on the page.** kahlus.com shows a price target and a "Work with us" page.
5. **The closed-loop sleep result is off the page.** It came from Kahlus-V2, now private. The mission line no longer says "closed-loop neurotechnology". The K7 figure assets were deleted. Bring them back if V2 goes public again.
6. **Public Kahlus-V1 README links to `kahlus-bench`, which is now private** (under the `ptlnextdoor` path). That link will 404 for visitors. Not changed here (out of scope).
7. **Research cards are now two** (Kahlus-V1, plasma). The brief allowed two to three.

## Proposed org settings (not applied)

- **Description:** Research in robotic cold plasma and EEG forecasting. We publish our methods, our code and the results that went against us.
- **Website:** https://kahlus.com
- **Location:** left blank until the captain gives one.

## Proposed pinned repositories (web UI, 6, all public)

1. Kahlus-V1 (leakage-controlled EEG forecasting, IECBES 2026)
2. kahlus-skills (agent skills)
3. subvox (silent speech from AirPods head motion)
4. sotto (coding agents steered by whispers and gestures)
5. mentra-eeg-miniapp (EEG readout on MentraOS glasses, synthetic signal)
6. hil-failure-modes (embedded failure test plans)

## Brand assets found

- Wordmark: `kahlus-wordmark-source.png` came from the Kahlus-V2 repo (now private). The draft banner already traces it into SVG paths in `profile/assets/`. The same wordmark PNGs also sit in `kahlus-research/client/public/`, also private. Keep the traced SVG as the public copy.
- Monogram "K" vector: https://kahlus.com/icon.svg
- Site look: black and white, JetBrains Mono and Instrument Sans, one muted pink accent (#eca8d6) on a small square marker. Off-white #ecebe7 and near-black #020204 appear in the site CSS.
