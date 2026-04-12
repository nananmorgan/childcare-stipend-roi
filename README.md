# Childcare Stipend ROI: A Data-Driven Business Case

## Overview
Childcare costs in the United States far exceed the national affordability benchmark of 7% of household income. This project builds a data-driven business case for employer-sponsored childcare stipends, targeting major tech employers in California and Washington. Using the National Database of Childcare Prices and a synthetic employer-sites dataset, the analysis quantifies affordability gaps at the county level, identifies priority pilot locations, and models the ROI of a monthly stipend program through retention savings and reduced absenteeism.

## Key Findings
- 99.1% of U.S. counties exceed the 7% childcare affordability benchmark, with a national median burden of 12.5%
- California and Washington rank among the top 3 states for median childcare burden (16.0% and 17.8%, respectively)
- A $550/month stipend brings 3 of 4 target hubs to or below the 7% benchmark
- ROI modeling shows net positive impact peaking in the $550–$600/month range, with a break-even point around $350/month
- Los Angeles and Sacramento emerge as top priority pilot locations (high burden + high female unemployment)

## Deliverables
- **PowerPoint Presentation** — A linear, slide-by-slide narrative for executive audiences walking through the problem, analysis, and recommendation
- **One-Page Executive Brief (PDF)** — A standalone summary with key visuals and the core recommendation, suitable as a handout or email attachment
- **Interactive Power BI ROI Dashboard** — Allows decision-makers to adjust assumptions (stipend amount, retention lift, replacement cost) and see real-time ROI projections with break-even analysis

## Data Sources
- **National Database of Childcare Prices** (U.S. Department of Labor) — County-level childcare costs, median household income, and demographic data
- **Synthetic employer-sites dataset** — Generated for scenario modeling with fields such as headcount, average salary, turnover rate, and uptake rate. Clearly labeled as synthetic throughout all materials

## Methods & Tools
- **Python** (pandas, matplotlib) for data cleaning, burden calculations, priority matrix, and visualization
- **Power BI** for the interactive ROI dashboard with adjustable sliders and break-even modeling
- **Gestalt design principles** and Cole Nussbaumer Knaflic's storytelling techniques applied throughout all visuals
- Left-aligned takeaway titles, neutral gray axes, single accent color for emphasis, direct labeling over legends

## Repository Contents
```
childcare-stipend-roi/
├── Nana_Noda-Morgan_DSC640_Milestone1_Analysis.ipynb   # Initial data analysis
├── Nana_Noda-Morgan_Mileston1_DataAnalysisX.ipynb      # Extended analysis notebook
├── DSC640-FinalProject-Milestone4.pdf                  # Final project write-up
├── PowerPoint_Presentation.pdf                         # Slide deck
├── Executive_Brief.pdf                                 # One-page executive summary
├── ROI_Dashboard.pbix                                  # Power BI dashboard (interactive)
├── ROI_Dashboard.pdf                                   # Dashboard screenshot/export
├── nationaldatabaseofchildcareprices.xlsx               # Source dataset
├── employer_sites_hr_synthetic.csv                     # Synthetic employer data
├── hub_stipend_needed_to_7pct.csv                      # Stipend gap calculations
├── slide2_state_burden_table.csv                       # State-level burden summary
├── Codes.xlsx                                          # Reference codes for dataset
└── README.md
```

## Ethical Considerations
The employer-sites dataset is synthetic and clearly labeled as such across all mediums. It was created for scenario testing and communication purposes only. County-level burden figures are derived directly from the National Database of Childcare Prices with light cleaning (data type fixes and duplicate removal). All assumptions — stipend amount, uptake rate, retention lift, and replacement cost — are transparently stated and adjustable in the Power BI dashboard.
