# PV-RR6 Calculator

**Dynamic prognostic model for polycythemia vera patients treated with ruxolitinib after hydroxyurea failure**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## Overview

Web-based calculator for the **PV-RR6 prognostic score**, developed by Palandri et al. (*Blood Advances*, 2026) within the PV-ARC study. The model provides dynamic, response-based risk stratification for patients with polycythemia vera (PV) treated with second-line ruxolitinib after hydroxyurea resistance or intolerance.

PV-RR6 integrates three readily available measures of disease control and treatment dose intensity, assessed over the first 6 months of ruxolitinib therapy, to predict **event-free survival (EFS)** — including thrombosis, hemorrhage, progression to post-PV myelofibrosis, or death — and to identify patients who may benefit from early treatment optimization.

It conceptually parallels the RR6 and iRR6 models developed in myelofibrosis, extending the dynamic risk-assessment framework to polycythemia vera.

---

## Score Variables

| Variable | Condition | Points |
|---|---|---|
| Spleen response | Absence of SR50 at **both** 3 and 6 months | +2.5 |
| Ruxolitinib dosing | <10 mg BID at ≥1 timepoint | +2.0 |
| Phlebotomy requirement | At 1 timepoint | +1.0 |
| Phlebotomy requirement | At ≥2 timepoints | +2.0 |

Total scores range from 0 to 6.5.

---

## Risk Categories

| Score | Category | 5-yr EFS | Median EFS | HR vs low |
|---|---|---|---|---|
| 0 | Low risk | 89.4% | Not reached | — |
| 1–2.5 | Intermediate risk | 71.0% | 7.72 years | 2.61 |
| ≥3 | High risk | 38.9% | 4.96 years | 6.15 |

PV-ARC cohort: n = 178 · median follow-up 3.50 years · log-rank p <0.001 · model significant after age adjustment (p = 0.001).

**EFS** = thrombosis, hemorrhage, progression to post-PV myelofibrosis, or death.

---

## Eligibility Criteria

The PV-RR6 model applies to patients with:

- Polycythemia vera (WHO 2022)
- Second-line ruxolitinib for ≥ 6 months, after hydroxyurea resistance or intolerance (ELN criteria)
- Available response data at baseline, 3 months, and 6 months (spleen, hematologic parameters, phlebotomy requirement, ruxolitinib dose)

---

## Deployment

Single self-contained HTML file — no framework, no backend, no dependencies (Google Fonts only).

```bash
git clone https://github.com/YOUR_USERNAME/pv-rr6-calculator
```

Deploy instantly on:
- **GitHub Pages** — Settings → Pages → Deploy from branch → main → Save
- **Netlify** — drag and drop the `index.html` file
- **Any static host** — upload the single file

> ⚠️ The file must be named **`index.html`** for GitHub Pages to serve it correctly.

---

## Reference

Palandri F, Dedola A, Caocci G, Rossi E, Elli EM, Sartor C, Latagliata R, Pugliese N, Morsia E, Binotto G, Mendicino F, Tieghi A, Benevolo G, Martino B, D'Addio A, Tiribelli M, Cilloni D, Crugnola M, Cavalca F, Scalzulli E, Lanza F, Pane F, Palumbo GA, Heidel FH, De Stefano V, Breccia M, Branzanti F. A dynamic prognostic model for polycythemia vera long-term outcomes in patients treated with ruxolitinib. *Blood Adv.* 2026 Jun 11:bloodadvances.2026020255.

doi: [10.1182/bloodadvances.2026020255](https://doi.org/10.1182/bloodadvances.2026020255) · PMID: 42275537 · PV-ARC Study (ClinicalTrials.gov NCT06134102)

---

## Intended Use

This tool is intended for use by qualified healthcare professionals as a clinical decision-support aid only. It does not substitute clinical judgment, institutional guidelines, or multidisciplinary discussion. Risk stratification should always be interpreted in the context of the individual patient's full clinical picture, cardiovascular risk profile, and treatment goals.

---

*PV-ARC Study · NCT06134102*
