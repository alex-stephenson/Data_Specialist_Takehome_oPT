# WANP Data Analysis Exercise

## Background

You are the data specialist for the **REACH Walloland mission**, a small nation based in sub-Saharan Africa.

REACH has been running a **longitudinal household, multisectoral needs assessment** for the past 18 months to assess population needs in the context of a long-running conflict:  **Walloland Assessment for Need Priorities (WANP)**. WANP is the **only representative household assessment in Walloland** and is a key tool for informing the humanitarian response.

Households who were in the initial assessment (cohort one) were asked if they could be contacted again, and remote assessments have been conducted at roughly 3 monthly intervals with the initial caseload. In November 2025 a new, in-person WANP assessment was conducted (cohort two), with the participants again being asked if they would agree to participate in future rounds. In January 2026, a remote assessment cohort 1 and cohort 2 was conducted. The aim of this exercise is to assess whether the combination of both cohorts in January 2026 was a statistically sound decision to make.

---

## Study Design

## Cohort Overview

| Feature | Cohort One | Cohort Two |
|--------|-----------|-----------|
| Initial assessment | June 2024 (in-person) | November 2025 (in-person) |
| Follow-up | Remote assessments every ~3 months | First follow-up in January 2026 |
| Re-contact consent | Yes | Yes |
| Sampling frame | Proportionate to population at governorate level | Proportionate to population at governorate level |
| Stratification | Building type | Building type |
| Margin of error | 3% | 3% |
| Confidence interval | 95% | 95% |



### January 2026 Remote Round
- The dataset included in this repository is the Jan 2026 assessment.
- This was a remote assessment conducted with **both cohorts**, using the sample questions for both cohorts.
- The Kobo tool in the repository includes:
  - Structural variables (demographics, location, etc.).
  - Outcome indicators.
- The Kobo tool can be used as a **codebook / data dictionary**.

---

## Dataset Description

- Columns to the right of `uuid` are **composite indicators** (pre-calculated).
- Assume these indicators are **correct**.

Some of the indicators you _may_ want to consider:

- `head_hh_gender` - Head of Household Gender
- `sampling_framework` - description of shelter type
- `governorate` - governorate
- `sum_hh_members` - total household size
- `hhs` – Household Hunger Score  
- `fcs` – Food Consumption Score  
- `ecfies` – Early Childhood Feeding Insecurity Score  
- `cohort` - Which cohort the HH originates from. Cohort One (June 2024) or Cohort Two (November 2025)

---

## Exercise Objective

Using the **January 2026 remote dataset**, assess whether:

> Combining Cohort One and Cohort Two into a **single analytical cohort** is a **statistically sound decision**.

Dataset provided:
- `Walloland_WANP_clean_data.xlsx`

You should consider:
- Are there been demographic, contextual or outcome indicators differences between these cohorts
- Can we still say that the combined sample is representative of the overall population
- Statistical comparisons between cohorts.
- Theoretical and sampling implications.

There is **no single correct answer**.  
You are expected to provide a **clear recommendation** with justification.

---

## Assumptions

- Population size and composition remain constant:
  - No net migration and Mortality rate = fertility rate 
  - Internal displacement has occurred.
- No survey weights available - Assume **unweighted analysis**.

---

## Inputs

You are provided with:
- The Kobo Survey
- January 2026 remote dataset.

---

## Outputs & Deliverables

### Time Expectation
- Aim to spend no more than three hours on this assessment. 
- You may be selective in scope, the answer doesn't need to be exhaustive.
- It is acceptable to state:
  > *“I would generalise this approach to X, Y, Z.”*

---

### GitHub Repository

You must submit:
- A GitHub repository containing:
  - All code (**R only**).
  - A `README.md` describing:
    - Methodology.
    - Recommendations.
    - Limitations and assumptions.
    

As instructed in the email, please email a link to your GitHub repository. Include  **Alex Stephenson** (alex.stephenson@impact-initiatives.org) in cc. 

---

## Interview

You should be prepared to:
- Walk through your analysis (max **10 minutes**).
- Answer questions from:
  - Technical stakeholders.
  - Non-technical stakeholders.

We are interested in seeing your code, your understanding of statistical and sampling techniques and methods, and your ability to communicate these findings to a range of stakeholders. 
