# Practice-Based Insights into Adult Genetics
### High Diagnostic Yield, Demographic Determinants, and Patterns of Test Utilization across 10,000 Patient Encounters

Jessica I. Gold, Yehuda Elkaim, Stephanie Asher, Zoe Bogus, Teresa Chai, Stacey Cohen, Courtney Condit, Isaac Elysee, Brielle N. Gehringer, Shannon M. Gray, Laura Hennessy, Emma Kennedy, Anna Raper, Maria Bonanni, Ala Streater, Eamon Toye, Colleen Kripke, Katherine L. Nathanson, Mersedeh Rohanizadegan, Staci Kallish, and Theodore G. Drivas\*

\*Corresponding author: theodore.drivas@pennmedicine.upenn.edu · Division of Translational Medicine and Human Genetics, Perelman School of Medicine at the University of Pennsylvania

---

## 🔗 Browse the full analysis

### **https://drivas-lab.github.io/medgenoutcomes-2025/**

The link above opens an interactive notebook containing every figure and supplementary figure in the manuscript, panel by panel and in manuscript order, together with the underlying statistics (unadjusted and covariate-adjusted), sortable summary tables, and the R code that generated each panel. Click **Show code** above any figure to see exactly how it was made. The notebook is a single self-contained page (≈56 MB), so allow a few seconds for the first load.

---

## Abstract

Genetic medicine has become a routine component of clinical care, yet the evidence guiding its implementation remains heavily weighted toward pediatric populations, with limited practice-level data to inform adult referral pathways, test selection, or service delivery. We analyzed eight years of electronic health record (EHR)-linked data from a high-volume adult genetics clinic (9,867 visits) within a major academic health system to define referral patterns, test utilization, and genetic testing outcomes across indications and demographic groups. While most visits were in-person and led by a genetics-trained physician, genetic counselor-only visits accounted for 12% of all encounters and telemedicine remained a substantial component of follow-up care, comprising 39% of follow-up visits from 2023 onward. Genetic testing was ordered for 52% of all new patients, with significant indication-specific variation in ordering propensity. Overall, 24% of all tests returned a diagnostic result. Diagnostic yield differed markedly by testing modality: exome sequencing yielded diagnoses in 40% of patients, whereas next-generation sequencing panels, the most frequently ordered testing type, yielded diagnoses in only 16%. Although diagnostic yield declined with increasing patient age, it remained above 17% in every age stratum, with the yield of exome/genome sequencing remaining above 30% across all age groups. Outcomes varied significantly by referral indication, with some indications yielding significantly high rates of pathogenic findings, and others more often yielding negative or uncertain results. Operational factors significantly shaped practice: test type and laboratory utilization shifted significantly over time in step with payer and testing lab policy changes. Together, these practice-based data establish adult genetics as a high-yield and important clinical domain. Our findings provide actionable evidence to inform age- and indication-aware triage, guide workforce planning, promote adult-focused practice guidelines, better inform payor reimbursement policies, and advance the integration of genomic medicine into routine adult patient care.

## What is in the notebook

| Section | Content |
|---|---|
| Figure 1 | Clinic demographics: patient catchment map, age, sex, race, ethnicity, provider type, visit type, insurance |
| Figure 2 | Referral indications, their change over time, and demographic composition by indication |
| Figure 3 | Genetic testing utilization by visit type, sex, age, race, and indication |
| Figure 4 | Testing modalities and laboratory utilization over time, with payer/policy inflection points |
| Figure 5 | Genetic testing results by sex, age, race, test type, and indication |
| Figure 6 | Variants identified, by gene and indication group |
| Figure 7 | Exome/genome sequencing results by patient and visit characteristics |
| Supplement | Visit types over time (S1), visits by specific indication (S2, Table S1), age distributions and results by indication group (S3), WES/WGS vs. other testing (S4) |

Every panel is shown with its manuscript legend; the statistics supporting each panel are directly beneath it in collapsible boxes.

## Repository contents

- `index.html` – the rendered notebook served at the link above
- `MedGenOutcomes2025_ForUpload.Rmd` – the R Markdown source that produces it

## Reproducing the analysis

The notebook knits from the `.Rmd` with R ≥ 4.x and the packages listed in the Session information section at the end of the rendered page (tidyverse, patchwork, DT, emmeans, nnet, ggmap, among others). Two values are read from environment variables at knit time and are not stored in the repository:

```
MEDGEN_DATA_PATH=path-to-data      # full path to the cleaned clinic data used in the analyses
STADIA_MAPS_KEY=your-key-here      # Stadia Maps API key, used only for the Figure 1A base map
```

Set them in `~/.Renviron`, restart R, and knit. The chunks stop with a clear message if either is missing.

## Data availability

The underlying dataset consists of patient-level electronic health record data from the Penn Medicine Adult Genetics Clinic and cannot be shared publicly. All aggregate results, statistics, and figure-level summaries are available in the notebook. Requests for collaborative access to de-identified data may be directed to the corresponding author and are subject to institutional review.

## Ethics

This study was conducted at the University of Pennsylvania and approved by the University of Pennsylvania Institutional Review Board (protocol 850058).

## Citation

If you use these results or this notebook, please cite the preprint:

> Gold JI, Elkaim Y, Asher S, Raper A, Condit C, Bogus Z, Elysee I, Hennessy L, Kennedy E, Chai T, Cohen S, Gehringer BN, Gray SM, Streater A, Toye E, Kripke C, Nathanson KL, Rohanizadegan M, Kallish S, Drivas TG. Practice-Based Insights into Adult Genetics: High Diagnostic Yield, Demographic Determinants, and Patterns of Test Utilization across 10,000 Patient Encounters. *medRxiv* 2026. doi: [10.1101/2025.10.09.25337579](https://doi.org/10.1101/2025.10.09.25337579)

```bibtex
@article{Gold2026AdultGenetics,
  title   = {Practice-Based Insights into Adult Genetics: High Diagnostic Yield, Demographic Determinants, and Patterns of Test Utilization across 10,000 Patient Encounters},
  author  = {Gold, Jessica I and Elkaim, Yehuda and Asher, Stephanie and Raper, Anna and Condit, Courtney and Bogus, Zoe and Elysee, Isaac and Hennessy, Laura and Kennedy, Emma and Chai, Teresa and Cohen, Stacey and Gehringer, Brielle N and Gray, Shannon M and Streater, Ala and Toye, Eamon and Kripke, Colleen and Nathanson, Katherine L and Rohanizadegan, Mersedeh and Kallish, Staci and Drivas, Theodore G},
  journal = {medRxiv},
  year    = {2026},
  doi     = {10.1101/2025.10.09.25337579},
  url     = {https://www.medrxiv.org/content/10.1101/2025.10.09.25337579v2}
}
```

The interactive notebook can be cited by its URL: https://drivas-lab.github.io/medgenoutcomes-2025/

## Contact

Theodore G. Drivas, MD PhD · theodore.drivas@pennmedicine.upenn.edu · [Drivas Lab](https://drivaslab.org/) · [BlueSky](https://bsky.app/profile/tdrivas.bsky.social)
