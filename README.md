# LA Health Expansion Index

Identify where new FQHC and community health centers are actually needed in Los Angeles.

---

## Overview
This project analyzes gaps in healthcare access across Los Angeles County and ranks ZIP codes based on unmet need.

Instead of relying on intuition or funding patterns, this approach uses data to highlight where new clinics would create the most impact.

---

## What This Project Does
- Map existing FQHC and community health clinic locations  
- Measure socioeconomic and population-level need using ACS data  
- Build a scoring system to rank all LA ZIP codes  
- Identify top areas for expansion  

---

## Model
This project uses a **weighted composite index model**.

- All variables are normalized to the same scale  
- Indicators are grouped into:
  - Need
  - Demand
  - Socioeconomic context  
- Each variable is weighted based on relevance  
- A clinic density penalty is applied to avoid over-served areas  

**Formula:**  
```
Need Index = Σ (wᵢ × xᵢ) − Clinic Density Penalty
```

This produces a continuous ranking across all ZIP codes.

---

## Data
- American Community Survey (ACS) 2011–2021  
- FQHC and non-profit community health clinic locations  
- NETS business data (NAICS healthcare categories)  

---

## Output
- Ranking of all LA County ZIP codes  
- Top 10 priority areas for new clinics  
- Map visualization (Tableau / Streamlit in progress)  

---

## Why This Matters
Healthcare access in Los Angeles is uneven. Some neighborhoods have multiple clinics, while others remain underserved.

This project provides a more structured, data-driven way to support FQHC and community health expansion decisions.

---

## Tools
- Python (pandas, sklearn)  
- Tableau  
- Streamlit  

---

