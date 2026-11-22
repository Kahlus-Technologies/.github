<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Kahlus-Technologies/.github/fm/kahlus-org-page/profile/assets/banner-dark.svg">
  <img src="https://raw.githubusercontent.com/Kahlus-Technologies/.github/fm/kahlus-org-page/profile/assets/banner-light.svg" alt="Kahlus Technologies" width="100%">
</picture>

<br>

**Research in robotic cold plasma and closed-loop neurotechnology.**<br>
We publish our methods, our code and the results that went against us.

<br>

[Website](https://kahlus.com) &nbsp;·&nbsp; [Plasma system](https://kahlus.com/plasma) &nbsp;·&nbsp; [Papers and talks](https://kahlus.com/research)

</div>

<br>

## Research

<table>
<tr>
<td>
<h3><a href="https://github.com/Kahlus-Technologies/Kahlus-V2">Kahlus-V2</a>: closed-loop sleep stimulation</h3>
Closed-loop sound stimulation can deepen slow-wave sleep, but a click just before a brief wake-up (an arousal) can wake the sleeper. This work replays a slow-wave click trigger on recorded nights and asks whether it fires right before scored arousals.
<br><br>
<b>Result.</b> On 5,768 SHHS-1 nights, the trigger fires before an arousal <b>5.01 times</b> as often as at matched moments from the same night (95% interval 4.83 to 5.18). On 2,031 sealed MESA nights, scored once, the ratio is 3.79. A fake trigger shifted in time gives about 1.0 in both.
<br><br>
<b>Limit.</b> This is a replay. No sound was played, so the result says nothing about what clicks do to sleep. It measures timing.
<br><br>
<a href="https://github.com/Kahlus-Technologies/Kahlus-V2/blob/main/docs/prereg/k1-k7.md">Preregistration</a> &nbsp;·&nbsp; <a href="https://github.com/Kahlus-Technologies/Kahlus-V2/releases/tag/v0.2-k7">Release v0.2-k7</a>
</td>
</tr>
</table>

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Kahlus-Technologies/.github/fm/kahlus-org-page/profile/assets/k7-trigger-timing-dark.png">
  <img src="https://raw.githubusercontent.com/Kahlus-Technologies/.github/fm/kahlus-org-page/profile/assets/k7-trigger-timing-light.png" alt="Relative risk of a brief wake-up within 3 seconds of a click trigger: 5.01 in SHHS-1 and 3.79 in sealed MESA. A time-shifted fake trigger gives 0.99 and 1.00." width="760">
</picture>

</div>

<table>
<tr>
<td>
<h3><a href="https://github.com/Kahlus-Technologies/Kahlus-V1">Kahlus-V1</a>: EEG forecasting under leakage control</h3>
Can past EEG predict future EEG in people the model has never seen? This work tests that with split rules fixed before any training.
<br><br>
<b>Result.</b> An early forecast score (Pearson r = 0.972) came from input and target windows that share almost all their samples. We retracted it. On strictly future samples and held-out subjects, the recurrent model did not beat a linear ridge baseline.
<br><br>
<b>Limit.</b> The remaining claim is the evaluation protocol that caught the error. It is not a forecasting-skill claim.
<br><br>
<a href="https://github.com/Kahlus-Technologies/Kahlus-V1#the-headline-result">Results</a> &nbsp;·&nbsp; <a href="https://kahlus.com/research">Paper (accepted, IECBES 2026)</a>
</td>
</tr>
</table>

<table>
<tr>
<td>
<h3><a href="https://kahlus.com/plasma">Robotic cold plasma</a>: a six-axis research prototype</h3>
A robot arm holds a cold-plasma torch at a set distance over curved surfaces, follows a planned path and logs every move. The arm is the open-source PAROL6 by Source Robotics. Kahlus built the control board, sensing, path planning and software.
<br><br>
<b>Result.</b> Position error stayed under <b>0.1 mm</b> across 50 commanded bench points. A thermal array cuts the discharge at 40 °C, and a hardware e-stop works outside the control software.
<br><br>
<b>Limit.</b> This is a research prototype. No treatment effect has been evaluated, and it is not cleared for clinical use.
<br><br>
<a href="https://kahlus.com/plasma">Plasma system</a>
</td>
</tr>
</table>

<br>

## How we work

#### Preregistered tests
We write down the question, the setting and the pass rule before the run. The preregistration file gets a SHA-256 hash, and every result file records it.

#### Sealed held-out data
A held-out cohort stays closed until the plan is frozen. It is then scored once. A guard in the code enforces the seal.

#### Leakage control
Features end at the prediction time. Every gain is compared with a time-shifted copy of the same features. If the copy gains too, the model learned the person and not the signal.

#### Results that went against us
We report nulls and retractions. Kahlus-V1 lost to simple baselines, and its README says so at the top.

<br>

## Papers and talks

<table>
<tr>
<td>
<b>Leakage-Controlled Evaluation of EEG Future-Window Forecasting in Held-Out Subjects</b><br>
<sub>Accepted. IEEE-EMBS IECBES 2026, Kuala Lumpur. Full conference paper, to be presented 9 to 11 December 2026. A. Patel, S. Zaidi, K. Garg.</sub>
</td>
</tr>
<tr>
<td>
<b>A Geometry-Aware Robotic Dosimetry Platform for Autonomous Cold Plasma Wound Therapy With Multimodal Closed-Loop Sensing</b><br>
<sub>Accepted. ASME IMECE 2026, Vancouver. Technical presentation, abstract only. A. Patel, S. Zaidi.</sub>
</td>
</tr>
<tr>
<td>
<b>Development of a Six-Degree-of-Freedom Robotic Platform for Automated DBD Plasma Wound Treatment</b><br>
<sub>Presented. IEEE ISEC 2026, Princeton, 14 March 2026. Two-page extended abstract and poster. A. Patel.</sub>
</td>
</tr>
</table>

<sub>"Accepted" means the venue accepted the work. Nothing here is called published until it appears in a proceedings index. <a href="https://kahlus.com/research">Full list</a></sub>

<br>

## Open source

**Research software**

- [kahlus-bench](https://github.com/Kahlus-Technologies/kahlus-bench): a leakage-sealed benchmark that scores neural-coupling estimators on synthetic systems with known directed information.
- [neuroforecast](https://github.com/Kahlus-Technologies/neuroforecast): directed-information graphs for multi-organ neural coupling, with a certified detection floor for each edge.
- [kahlus-research](https://github.com/Kahlus-Technologies/kahlus-research): deterministic replay of public biosignal recordings with injected faults. Actuation is disabled.

**Agent skills**

- [kahlus-skills](https://github.com/Kahlus-Technologies/kahlus-skills): five skills for research repo style, publication figures and removing AI tells from prose. They work with Claude Code, Codex and Jcode.

**Side projects**

- [Subvox](https://github.com/Kahlus-Technologies/subvox): tests whether AirPods head motion can carry silently mouthed words (macOS).
- [Sotto](https://github.com/Kahlus-Technologies/sotto): a hackathon project that steers coding agents with whispers and head gestures.
- [mentra-eeg-miniapp](https://github.com/Kahlus-Technologies/mentra-eeg-miniapp): an EEG state readout on MentraOS glasses. The demo signal is synthetic.
- [hil-failure-modes](https://github.com/Kahlus-Technologies/hil-failure-modes): six hardware-in-the-loop test plans for embedded failures. Bench runs come next.

<br>

<div align="center">

<a href="https://kahlus.com">kahlus.com</a><br>
<sub>Nothing here is cleared for clinical use.</sub>

</div>
