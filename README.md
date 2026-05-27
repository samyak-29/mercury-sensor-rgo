# 🧪 T&C-rGO Mercury Ion Sensor
> Thiol and carboxylic co-functionalized reduced graphene oxide device for highly selective ppb-level mercury ion detection in water  
> **📄 Submitted to IEEE Sensors Journal — Under Minor Revision (2026)**

---

## 📌 Overview

Mercury (Hg²⁺) is one of the most toxic heavy metals — even trace amounts above **6 ppb** in water can cause neurological damage, kidney failure, and developmental disorders. Conventional detection methods (AAS, ICP-MS) are expensive, lab-bound, and require skilled operators, making on-site monitoring impractical.

This project presents a **low-cost, portable, resistive sensor** based on thiol and carboxylic co-functionalized reduced graphene oxide (**T&C-rGO**) that detects mercury ions in water at the **parts-per-billion (ppb) level** with high sensitivity, selectivity, and long-term stability.

---

## ⚡ Key Results

| Parameter | Value |
|---|---|
| Detection range | 2 ppb – 1 ppm |
| Sensitivity at 2 ppb | **100.1 µA/ppb** |
| Sensitivity at 1 ppm | 5.35 µA/ppb |
| Response time | **19 seconds** |
| Operating voltage | 2 V (low power) |
| Stability | **40 days** (no significant drift) |
| Selectivity | Dominant response to Hg²⁺ vs Cd²⁺, Pb²⁺, As³⁺, Na⁺, K⁺ |

---

## 🔬 Sensing Principle

The sensing mechanism relies on the **strong affinity between mercury ions and thiol (–SH) groups** via Hg–S bond formation:

1. Cysteine (amino acid) is used to functionalize rGO sheets
2. The **amine (–NH₂) group** of cysteine binds to the –OH groups on the rGO basal plane
3. This exposes the **thiol (–SH) and carboxyl (–COOH) groups** to incoming mercury ions
4. Hg²⁺ binding causes **electron transfer** from mercury to T&C-rGO
5. This reduces hole concentration in the sensing layer → **measurable decrease in conductivity**

```
Hg²⁺ + –SH (T&C-rGO) → Hg–S bond → ↓ conductivity → ↑ resistance → measurable signal
```

---

## 🛠️ Device Fabrication

### Step 1 — Synthesis of T&C-rGO
- Graphene oxide (GO) synthesised via **modified Hummers method**
- 2g NaNO₃ + 4g graphite in 92ml H₂SO₄ (98%), stirred 15h
- KMnO₄ added slowly, followed by 160ml DI water (exothermic → 98°C)
- Solution centrifuged and washed with 4% HCl and DI water
- **10mg cysteine** added to 100ml GO, stirred 2h, ultrasonicated 1h
- Heated at **85°C for 4 hours** → T&C-rGO formed

### Step 2 — Device Fabrication
- Substrate: n<100> silicon wafer (resistivity 4–20 Ω·cm)
- 120 nm SiO₂ grown by thermal oxidation
- **20nm Ti** sputtered as adhesion layer
- **180nm Au** sputtered and lithographically patterned
- Electrode channel gap: **40 µm**, width: **220 µm**
- T&C-rGO deposited by **drop-casting**

### Step 3 — Characterisation
| Technique | Purpose |
|---|---|
| FESEM | Surface morphology — sheet-like structure, 5–25 µm dimensions |
| HRTEM | Lattice fringes — d-spacing 0.34 nm (≈ pristine graphene 0.36 nm) |
| XRD | GO peak at 10.48° (001); T&C-rGO broad peak at 24.57° (002) |
| FTIR | O–H (3000–3500 cm⁻¹), S–H (2550–2600 cm⁻¹), N–H (1580–1650 cm⁻¹) |

---

## 📊 Results

### I-V Characteristics — Hg²⁺ Detection (2 ppb to 1 ppm)
Clear stepwise decrease in current with increasing Hg²⁺ concentration, confirming concentration-dependent resistive response.

![I-V Characteristics](results/mercury_iv.jpg)

---

### Dynamic Response — Real-Time Monitoring
Base current at 2V: **1.8 mA**. After 20 ppb Hg²⁺ exposure: drops to **0.6 mA**. Response time: **19 seconds**.

![Dynamic Response](results/ivt_mercury.jpg)

---

### Selectivity — Hg²⁺ vs Other Metal Ions
T&C-rGO shows dominant response (~92%) to Hg²⁺ at 1 ppm, with significantly lower response to Cd²⁺, Pb²⁺, As³⁺, Na⁺ and K⁺.

![Selectivity](results/Selectivity_towards_Hg.jpg)

---

### Sensitivity — dI/dC vs Concentration
Hg²⁺ sensitivity of **100 µA/ppb** at 2 ppb — far exceeding all other ions tested.

![Sensitivity](results/Sensitivity_TC-rGO.jpg)

---

### Stability — 40 Days
Sensitivity remains stable at ~100 µA/ppb over 40 days under identical experimental conditions — zero significant drift.

![Stability](results/stability.jpg)

---

### Material Characterisation

**XRD** — Sharp GO peak at 10.48° (001) confirms oxidation. Broad T&C-rGO peak at 24.57° (002) confirms successful reduction and functionalisation.

![XRD](results/cysteine_rgo_XRD.jpg)

**FTIR** — Confirms presence of O–H, S–H, N–H and N=C=S functional groups, validating successful cysteine functionalisation.

![FTIR](results/FTIR__1_.jpg)

---

## 📋 Instruments Used

| Instrument | Purpose |
|---|---|
| Probe Station (PLV 50) | Electrical characterisation |
| Semiconductor Parameter Analyser (B1500) | I-V and I-t measurements |
| FESEM | Surface morphology |
| HRTEM | Lattice structure and d-spacing |
| XRD (Cu Kα₁, λ = 1.54 Å) | Crystallographic analysis |
| FTIR | Functional group identification |

---

## 📁 Repository Structure

```
mercury-sensor-rgo-ieee/
├── results/
│   ├── mercury_iv.jpg           # I-V characteristics (2ppb–1ppm)
│   ├── ivt_mercury.jpg          # Dynamic real-time response
│   ├── Selectivity_towards_Hg.jpg  # Selectivity bar chart
│   ├── Sensitivity_TC-rGO.jpg   # Sensitivity vs concentration
│   ├── stability.jpg            # 40-day stability plot
│   ├── cysteine_rgo_XRD.jpg     # XRD pattern GO vs T&C-rGO
│   └── FTIR__1_.jpg             # FTIR spectra
└── README.md
```

---

## 📄 Publication

> **Khatod S.\*, Rawat P.\*, Sundereswaran U M., Nikhil, Mandal S., Sett A.**  
> *"Thiol and carboxylic co-functionalized graphene-based device for highly selective mercury ion detection in water"*  
> **IEEE Sensors Journal** — Under Minor Revision (2026)  
> *\* Equal contribution, Co-First Authors*

---

## 👥 Authors

**Samyak Khatod** (Co-First Author)  
B.Tech, Electronics & Communication Engineering  
SRM Institute of Science and Technology, Kattankulathur  
📧 khatodsamyak50@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/samyak-khatod) | [GitHub](https://github.com/samyak-29)

**Supervised by:** Dr. Avik Sett (SRMIST & TU Delft, Netherlands)

---

## 🌍 Impact

This sensor addresses **UN SDG 6 (Clean Water and Sanitation)** by providing an affordable, portable alternative to laboratory-based heavy metal detection. The device operates at only 2V, making it suitable for battery-powered, field-deployable water quality monitoring systems.

---

## ⚠️ Note

This repository contains research results and characterisation data. The full paper is currently under peer review at IEEE Sensors Journal. Code and raw data will be updated upon publication.
