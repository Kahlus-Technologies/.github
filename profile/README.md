<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Kahlus-Technologies/.github/fm/kahlus-org-page/profile/assets/banner-dark.svg">
  <img src="https://raw.githubusercontent.com/Kahlus-Technologies/.github/fm/kahlus-org-page/profile/assets/banner-light.svg" alt="Kahlus Technologies" width="100%">
</picture>

<br>

**Research in robotic cold plasma and EEG forecasting.**<br>
We publish our methods, our code and the results that went against us.

<br>

[Website](https://kahlus.com) &nbsp;·&nbsp; [Plasma system](https://kahlus.com/plasma) &nbsp;·&nbsp; [Papers and talks](https://kahlus.com/research)

</div>

<br>

## Research

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
<a href="https://github.com/Kahlus-Technologies/Kahlus-V1#the-headline-result">Results</a> &nbsp;·&nbsp; <a href="https://kahlus.com/research">Paper (IECBES 2026)</a>
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

#### Split rules first
We fix the train, validation and test splits before preprocessing and before any model runs. Held-out subjects, sites and datasets stay out of training.

#### Leakage audits
We check for reused records, overlapping held-out groups, repeated windows and forbidden target metadata. These audits caught an error in our own first result.

#### Strong baselines
Every model is scored against simple baselines such as persistence and linear ridge regression. A model that does not beat them says so in its README.

#### Results that went against us
We report nulls and retractions. Kahlus-V1 retracted its headline forecast score, and its README says so at the top.

<br>

## Papers and talks

<table>
<tr>
<td>
<b>Leakage-Controlled Evaluation of EEG Future-Window Forecasting in Held-Out Subjects</b><br>
<sub>Published. IEEE-EMBS IECBES 2026, Kuala Lumpur. Full conference paper, to be presented 9 to 11 December 2026. A. Patel, S. Zaidi, K. Garg.</sub>
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

<sub>"Accepted" means the venue accepted the work. "Presented" means it was given. <a href="https://kahlus.com/research">Full list</a></sub>

<br>

## Open source

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
