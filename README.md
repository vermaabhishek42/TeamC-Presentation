# TeamC Presentation
---
title: "Not Just Replicated — Refined: Figure A9B in R"
author: "Abishek Verma"
date: "June 13, 2025"

---

## Project Scope

-   Reproduced **Figure A9B** from the assigned academic paper
-   Transitioned from **Stata .gph** to **RStudio (ggplot2)**
-   Replicated female model results showing R² progression across six specifications

------------------------------------------------------------------------

## Original Output (Stata)

-   Figure A9B in the paper was generated using Stata's `.gph` graphing
-   Visual quality was limited, and metadata extraction was necessary
-   Our task: **rebuild this figure** using clean, reproducible R code

------------------------------------------------------------------------

## Refined Figure A9B: Original vs RStudio Version

| Original (Stata .gph)   | Recreated in R (ggplot2)                          |
|-------------------------------------|-----------------------------------|
| ![](images/Fig_A9B.png) | ![](images/Screenshot 2025-06-11 at 17.53.12.png) |

------------------------------------------------------------------------

## Technical Hurdles

- `.gph` file required manual decoding — no access to raw dataset
- Values extracted from graph metadata instead of numeric source
- `ggplot2` styling rebuilt from scratch to exceed original visual quality
- Manual adjustments needed:
  - Label rotation
  - Text placement
  - Axis scaling
  - Legend removal for clarity

---

## Outcome

- Visually polished, slide-ready, and appropriate for academic use
- Fully reproducible in R using a lightweight and modular code block
- Custom styling improves clarity without losing original meaning

---

## Functions Used in This Replication

- `ggplot()` – base plotting function  
- `geom_col()` – creates bar chart columns  
- `geom_text()` – adds R² labels on top of bars  
- `scale_fill_manual()` – custom color palette  
- `theme_minimal()` – clean background  
- `labs()` – axis titles and plot title  
- `factor()` – for ordering model components

> Code structured to be reusable and modular for future replications

---

## References

- R Core Team (2025). *R: A language and environment for statistical computing.*
- Wickham et al. (2023). *ggplot2: Elegant graphics for data analysis.*
- RColorBrewer: Color palettes used for improved visuals
  

---

## Thank You!

> Questions? Comments?  
> This replication was prepared using **RStudio, Quarto**   
> Slide created by Abishek Verma | June 2025
