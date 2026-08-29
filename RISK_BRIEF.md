# Cyclone Risk Assessment - Coastal Odisha Belt

**Peril:** Tropical cyclone (wind only)
**Domain:** Coastal Odisha belt, 17-22°N / 82-88°E
**Basis:** Modelled economic loss on a built-asset exposure proxy
**Date:** 28-08-2026
**Prepared by:** Navneet Krishnan

---

## 1. Summary

Total modelled exposure across the coastal Odisha belt is **₹144.86B**. Expected annual loss from tropical cyclone wind is ₹1.533B, or 1.06% of exposure. This is relatively high for a wind-only estimate, reflecting the steep Odisha-specific vulnerability curve and the concentration of exposure within the coastal study domain. The estimate is highly sensitive to the assumed building vulnerability, which is the dominant source of uncertainty in the analysis.

---

## 2. Key figures

| Measure | Value | Plain meaning |
|---|---|---|
| Exposure | ₹144.86B | Total asset value in the modelled domain |
| Average Annual Loss | ₹1.533B | Long-run average cost per year |
| 1-in-100 year loss (occurrence) | ₹32.81B | Loss from a single event at approximately the 1-in-100 OEP level |
| 1-in-100 year loss (annual aggregate) | ₹35.22B | Total annual loss at approximately the 1-in-100 AEP level |
| 1-in-100 TVaR | ₹47.49B | Average loss *given* a 1-in-100 year is exceeded |

![Baseline Cyclone Loss Exceedance Curves](outputs/figures/oep_aep_curve.png)

*Figure 1. Baseline occurrence and aggregate cyclone loss exceedance curves. The 100-year occurrence and aggregate losses are approximately ₹32.81B and ₹35.22B respectively; tail estimates are increasingly sampling-sensitive beyond 1-in-50 years.*

---

## 3. What drives the risk

- Loss is highly spatially concentrated: the five highest-AAL centroids account for approximately **56% of total modelled AAL**, with the largest concentrations around **84.75-85.75°E, 19.25-20.25°N** and a secondary concentration around **86.0-86.5°E, 20.25-20.50°N**.
- Cyclones affect the domain roughly **2.2 times per year**, but only about **0.26 per year produce measurable loss** on the modelled exposure. Risk is therefore characterised by rare, severe outcomes rather than frequent attritional losses.
- The relationship between wind speed and damage is strongly non-linear: a **10% increase in
wind intensity raises expected annual loss approximately 40%**.
- Maximum wind intensity has only a moderate association with event loss (**Pearson r = 0.454**). The largest losses are concentrated among **Fani- and Phailin-derived tracks**, indicating that the spatial relationship between cyclone tracks and exposed value matters alongside storm intensity.

---

## 4. Reinsurance structure

| Layer | Structure | Expected loss to layer | Technical RoL | Attachment prob. |
|---|---|---|---|---|
| 1 | ₹10B xs ₹12B | ₹265.05M | 2.65% | 3.689% |
| 2 | ₹15B xs ₹22B | ₹202.45M | 1.35% | 1.848% |
| 3 | ₹20B xs ₹37B | ₹85.60M | 0.43% | 0.836% |

Attachment is anchored near the 1-in-25 year loss, so the cedant retains losses expected
roughly once a generation and transfers severity above that point. Technical RoL declines up the tower as higher layers become progressively less likely to attach.

---

## 5. Confidence and caveats

**Wind only.** Storm surge and rainfall flooding are excluded. For this coastline these are
material loss drivers, so the figures above should be read as a **partial view of cyclone
risk, not a total one.** A back-test against Cyclone Fani (2019) gave a modelled wind loss of
₹46.91B against ₹93.36B of reported economic loss. The difference is consistent with the
model's wind-only scope and proxy exposure base, but this is a directional back-test rather
than a calibration target: the reported figure also covers asset classes and loss types
outside the model.

**Vulnerability is the dominant uncertainty.** Substituting an alternative, US-calibrated
damage function reduces expected annual loss by a factor of approximately 11.4x, and moves
layer pricing correspondingly. Regional vulnerability calibration would likely reduce this uncertainty more than further refinement of the current hazard model

**Tail estimates are sampling-limited.** Estimates become increasingly sampling-sensitive
beyond 1-in-50 years: the 1-in-100 figure rests on approximately 12 modelled events and the
1-in-200 on 6. These should be treated as indicative. Statistical extrapolation of the tail
was tested and rejected because the available exceedances did not support a sufficiently stable parametric fit.

**Economic, not insured, loss.** Figures represent total economic damage to modelled assets,
not insured loss. Insurance penetration and policy terms are not represented in the model, so insured loss would be expected to differ materially from these economic-loss estimates.

---

## 6. What I would want before pricing this

1. A stratified building-type inventory for the domain, to apply the vulnerability curve by
   construction class rather than as a single blended function
2. Storm surge and inland flood modules, to move from a wind-only to a multi-peril view
3. Actual portfolio exposure with insured values and policy terms, replacing the LitPop proxy
4. Claims data from recent events (Fani, Yaas) to calibrate and validate the damage function

---

