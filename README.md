# Surface Undulation via Laser Texturing and Its Effect on Wettability

> **Altering surface morphology of SrTiO₃(001) and Si(001) substrates using a KrF excimer laser and analysing the resulting changes in surface wettability.**

---

## Table of Contents

- [Overview](#overview)
- [Scientific Background](#scientific-background)
- [Objectives](#objectives)
- [Materials](#materials)
- [Experimental Setup](#experimental-setup)
- [Methodology](#methodology)
- [Characterisation Techniques](#characterisation-techniques)
- [Key Results](#key-results)
- [Literature Context](#literature-context)
- [References](#references)

---

## Overview

This project investigates how controlled laser-induced surface texturing modifies the surface morphology of epitaxial **SrTiO₃(001) (STO)** and **Si(001)** substrates, and how those morphological changes affect the surface **wettability** as quantified by the **Water Contact Angle (WCA)**. Surface texturing is performed using the **KrF excimer laser (248 nm)** available in a **Pulsed Laser Deposition (PLD)** system. The resulting microstructures are characterised with **Atomic Force Microscopy (AFM)** and **optical microscopy**, and wettability is measured using the **sessile drop method** analysed in ImageJ.

The central finding is that laser irradiation at controlled fluence and pulse count produces well-defined periodic ripple microstructures on the STO surface, measurably increasing surface roughness and altering the wettability behaviour of the substrate.

---

## Scientific Background

The wettability of a solid surface is one of its most fundamental properties and is quantified by the **Water Contact Angle (WCA)**:

| WCA Range | Classification |
|-----------|---------------|
| < 10° | Superhydrophilic |
| 10° – 90° | Hydrophilic |
| 90° – 150° | Hydrophobic |
| > 150° | Superhydrophobic |

Wettability is governed by two factors: **surface chemistry** and **surface morphology (roughness)**. On an ideal smooth surface, the equilibrium contact angle is given by **Young's equation**:

$$\cos\theta_Y = \frac{\gamma_{SV} - \gamma_{SL}}{\gamma_{LV}}$$

where γ_SV, γ_SL, and γ_LV are the solid–vapour, solid–liquid, and liquid–vapour interfacial energies respectively.

For real rough surfaces, two wetting models apply:

- **Wenzel model** — liquid fills the surface asperities (homogeneous wetting). Roughness amplifies the intrinsic wetting tendency: hydrophilic surfaces become more hydrophilic and hydrophobic surfaces become more hydrophobic.
- **Cassie–Baxter model** — air is trapped beneath the droplet (heterogeneous wetting). This leads to apparent contact angles higher than predicted by Wenzel and is the basis of superhydrophobicity.

By engineering surface roughness at the micro- and nanoscale via laser texturing, wettability can be tuned across the full spectrum — from superhydrophilic to superhydrophobic — **without altering surface chemistry**.

---

## Objectives

1. Use Pulsed Laser Deposition (PLD) with a KrF excimer laser to create controlled microstructures on STO(001) and Si(001) surfaces.
2. Optimise laser parameters (fluence, pulse number, repetition rate) to obtain reproducible periodic ripple structures.
3. Characterise surface roughness before and after laser irradiation using AFM and optical microscopy.
4. Measure and compare the water contact angle of pristine and laser-irradiated surfaces using the sessile drop method.
5. Establish the relationship between laser-induced surface undulation and wettability change on perovskite oxide substrates.

---

## Materials

| Sample | Dimensions | Quantity | Notes |
|--------|-----------|----------|-------|
| Epitaxial SrTiO₃(001) — STO | 5 mm × 5 mm | 3 | Perovskite oxide, atomically flat as-received |
| Si(001) | 10 mm × 10 mm | 3 | Reference substrate, well-characterised laser response |

**Sample preparation:**
- Cleaned sequentially with **isopropanol (IPA)**, **acetone**, and **deionised (DI) water** in an ultrasonic bath.
- Dried with dry nitrogen.
- STO(001) samples were mounted on top of Si(001) substrates using **silver paste** on the target holder, ensuring good thermal contact and mechanical stability inside the PLD chamber.

---

## Experimental Setup

### Pulsed Laser Deposition (PLD) System

The PLD system was used for laser texturing (not thin-film deposition). Key components:

| Component | Role |
|-----------|------|
| **KrF Excimer Laser** (248 nm, ~30 ns pulse width) | Primary irradiation source for surface texturing |
| **Vacuum Chamber** | Houses target/substrate; working area for experiment |
| **Rotary Pump** | Creates initial rough vacuum |
| **Turbo Molecular Pump** | Achieves high vacuum (~10⁻⁶ mbar) |
| **Pressure Gauges** | Monitor chamber pressure throughout |
| **ACTC Controller** | Sets target frequency, pulse count, beam positioning |
| **Laser Controller** | Sets laser energy (mJ), repetition rate (Hz) |

The laser is mounted **externally** to the chamber, which allows a wide dynamic range of operating pressures (10⁻¹⁰ to 10² Torr) and enables introduction of reactive gases without modifying the laser hardware.

### Laser Parameters Used

| Run | Pulses | Repetition Rate | Energy | Attenuation | Notes |
|-----|--------|-----------------|--------|-------------|-------|
| Run 1 | 4000 | 10 Hz | 250 mJ | None | Over-ablation — eyeball crater formed |
| Run 2 | 1000 | 1 Hz | 250 mJ | Metallic mesh grid | Clean periodic ripples formed |
| Run 3 | 1000 | 1 Hz | 250 mJ | Metallic mesh grid | Reproducibility run — identical to Run 2 |

> **Key insight:** Using a **metallic mesh grid** to attenuate the beam and remove the rotation/rastering mode was critical for producing clean, reproducible periodic microstructures rather than deep ablation craters.

---

## Methodology

### Laser Texturing Procedure

1. Mount samples on target holder and install in PLD chamber.
2. Pump down with rotary pump to rough vacuum, then engage turbo molecular pump to reach high vacuum (~10⁻⁶ mbar).
3. Set laser parameters (energy: 250 mJ; repetition rate: 1 Hz; pulse count: 1000) using the laser and ACTC controllers.
4. Irradiate the sample surface with the KrF excimer laser pulses.
5. Vent the chamber, remove samples.
6. Proceed to characterisation.

### Water Contact Angle Measurement (Sessile Drop Method)

1. Place the laser-irradiated sample on a glass slide in a well-lit, low-humidity environment.
2. Position a camera horizontally at the same level as the sample surface.
3. Use a ~30G syringe filled with DI water to deposit a small droplet (~3–5 µL) onto the surface.
4. Record a video and extract a clear side-profile frame showing the droplet–surface interface.
5. Import the frame into **ImageJ** with the **Contact Angle plugin**.
6. Convert to 8-bit greyscale; mark the two baseline points along the solid–liquid interface.
7. Mark ≥3 points along the droplet curvature.
8. Click **Manual** and then **Results** — ImageJ fits the drop curvature and returns θ values.
9. Compute **WCA = 180° − θ**.

---

## Characterisation Techniques

### Atomic Force Microscopy (AFM)

- **Mode:** Tapping (intermittent contact) mode
- **Purpose:** Quantify surface roughness parameters (Ra, Rq/Rms) before and after laser irradiation on the same sample areas.
- **Scan areas:** 3 µm × 3 µm and 5 µm × 5 µm
- **Output:** Height images (2D and 3D), Ra and Rms roughness values, direct before/after comparison.

### Optical Microscopy

- **Mode:** Reflected-light (epi-illumination)
- **Purpose:** Visualise the spatial distribution of laser-induced microstructures, ripple periodicity, pit dimensions, and beam footprint.
- **Magnifications used:** 5× → 100×
- **Image analysis:** ImageJ used to measure ripple width distributions and pit feature area distributions.

### Sessile Drop / Contact Angle Goniometry

- **Method:** Static sessile drop with DI water (~3–5 µL droplet)
- **Analysis:** ImageJ Contact Angle plugin
- **Output:** Static WCA for bare and laser-irradiated surfaces

---

## Key Results

### Surface Morphology

| Condition | Observation |
|-----------|-------------|
| **4000 pulses @ 10 Hz (no mesh)** | Eyeball-like crater at beam centre; excessive ablation; aperiodic microstructures at periphery |
| **1000 pulses @ 1 Hz (with mesh)** | Clean periodic ripple microstructures; spatial distribution consistent with Gaussian beam profile |
| **Reproducibility (Run 3, same params)** | Identical ripple structures confirmed; experiment is reproducible |

**Spatial structure of irradiated area (1000 pulses, mesh):**
- **Centre:** Periodic ripple structures (laser-induced periodic surface structures, LIPSS)
- **Periphery:** Aperiodic microstructures
- **Outer edge:** Boundary between irradiated and unirradiated (pristine) surface

### AFM Roughness

| Sample | Ra (nm) | Rms (nm) |
|--------|---------|----------|
| Bare STO(001) | 0.378 | 0.232 |
| Laser-irradiated STO | 11.68 | 3.156 |


### Wettability

| Sample | WCA (°) | Classification |
|--------|---------|---------------|
| Bare STO(001) | [X] | — |
| Laser-irradiated STO | [Y] | — |


---

## Literature Context

This work is informed by several key studies demonstrating the power of laser texturing to control wettability:

| Study | Material | Laser | WCA Change | Key Finding |
|-------|----------|-------|-----------|-------------|
| Liu et al. (2010) [1] | PVDF polymer | KrF excimer (248 nm) | 53° → 170° | Superhydrophobicity via wall-like structures + C–CF₂/C–F surface chemistry |
| Wang et al. (2009) [2] | Si(001) | UV DPSS (355 nm) | 64.2° → 97.5° | Laser pit parameters directly control contact angle |
| Ha (2024) [3] | Copper | Ti:sapphire femtosecond | > 90° → < 1° | LIPSS → superhydrophilicity; spontaneous hydrophobic transition in air over ~10 days |
| Sohrabi et al. (2022) [6] | Polycarbonate | KrF excimer (248 nm) | 91° → > 150° | Superhydrophobicity + antibacterial properties from ns laser above ablation threshold |
| Luo et al. (2010) [7] | Stainless steel | KrF excimer (248 nm) | 68.5° → 130° | Groove pattern geometry (b/a ratio) directly controls WCA via Cassie–Baxter model |
| Zorba et al. (2006) [8] | Si | Ti:sapphire femtosecond | 66° → > 130° | Two-lengthscale micro/nano patterning; no coating required |


---

## References

```
[1] Y. Liu, Q. Wei, Y. Jiang, and Z. Nie, "Increasing the hydrophobic property of poly
    (vinylidene fluoride) by KrF excimer laser irradiation," Applied Physics Letters,
    vol. 96, no. 25, p. 231109, 2010. https://doi.org/10.1063/1.3452343

[2] X. C. Wang, L. Y. L. Wu, Q. Shao, and H. Y. Zheng, "Laser micro structuring on a
    Si substrate for improving surface hydrophobicity," Journal of Micromechanics and
    Microengineering, vol. 19, no. 8, p. 085025, 2009.
    https://doi.org/10.1088/0960-1317/19/8/085025

[3] J. Ha, "Superhydrophilic Surface Creation and Its Temporal Transition to Hydrophobicity
    on Copper via Femtosecond Laser Texturing," Coatings, vol. 14, no. 9, p. 1107, 2024.
    https://doi.org/10.3390/coatings14091107

[4] N. A. Shepelin et al., "A practical guide to pulsed laser deposition," Chemical
    Society Reviews, vol. 52, no. 7, pp. 2294–2321, 2023.
    https://doi.org/10.1039/D2CS00938B

[5] A. V. Ragutkin et al., "Creation of Hydrophobic Functional Surfaces of Structural
    Materials on the Basis of Laser Ablation (Overview)," Thermal Engineering,
    vol. 69, no. 6, pp. 429–449, 2022. https://doi.org/10.1134/S0040601522050056

[6] S. Sohrabi, H. Pazokian, B. Ghafary, and M. Mollabashi, "Superhydrophobic-antibacterial
    polycarbonate fabrication using excimer laser treatment," Optik, vol. 262, p. 169377,
    2022. https://doi.org/10.1016/j.ijleo.2022.169377

[7] B. H. Luo, P. W. Shum, Z. F. Zhou, and K. Y. Li, "Preparation of hydrophobic surface
    on steel by patterning using laser ablation process," Surface & Coatings Technology,
    vol. 204, pp. 1180–1185, 2010. https://doi.org/10.1016/j.surfcoat.2009.10.043

[8] V. Zorba et al., "Making silicon hydrophobic: wettability control by two-lengthscale
    simultaneous patterning with femtosecond laser irradiation," Nanotechnology,
    vol. 17, pp. 3234–3238, 2006. https://doi.org/10.1088/0957-4484/17/13/026
```

---

*This project was conducted as part of a research internship. Characterisation data (AFM roughness values and quantitative WCA measurements) will be updated upon completion of final analysis.*
