# Childcare Stipend ROI: A Data-Driven Business Case

## Overview
Childcare costs in the U.S. far exceed the national affordability benchmark of 7% of household income. This project builds a data-driven business case for employer-sponsored childcare stipends, targeting major tech employers in California and Washington. Starting from the National Database of Childcare Prices, the analysis quantifies affordability gaps at the county level, identifies the best pilot locations using a priority matrix, and models the ROI of a monthly stipend program through retention savings and reduced absenteeism. Findings are delivered in three formats designed for executive audiences.

## Key Findings
- 99.1% of U.S. counties exceed the 7% childcare affordability benchmark, with a national median burden of 12.5%
- California and Washington rank in the top 3 states for median childcare burden (16.0% and 17.8%)
- Major employer hubs including Los Angeles, San Francisco, Sacramento, and King County sit 6 to 11 percentage points above the 7% benchmark
- Los Angeles and Sacramento land in the "high burden and high unemployment" quadrant of the priority matrix, making them the strongest candidates for a pilot
- The net impact curve peaks in the $550 to $600/month range, with a break-even point around $350/month
- At $550/month, 3 of 4 target hubs drop to 7% or below childcare burden

## Deliverables
- **PowerPoint Presentation**: A linear, slide-by-slide narrative for executive audiences, with each slide building the case for approving the pilot program
- **One-Page Executive Brief (PDF)**: A standalone summary with key visuals and the core recommendation, designed to stand alone without a presenter
- **Interactive Power BI ROI Dashboard**: Allows decision-makers to adjust assumptions (stipend amount, retention lift, uptake rate, replacement cost) and see real-time ROI and break-even projections

## Data Sources
- **National Database of Childcare Prices** (U.S. Department of Labor): County-level childcare costs, median household income, and female unemployment data
- **Synthetic employer-sites dataset**: Created for scenario modeling with fields including headcount, average salary, turnover rate, uptake rate, and average children per parent. Clearly labeled as synthetic throughout all materials to avoid confusion with observed outcomes

## Methods and Tools
- **Python** (pandas, numpy, matplotlib) for data cleaning, burden calculations, state and county analysis, priority matrix, stipend gap calculations, and ROI modeling
- **Power BI** for the interactive dashboard with adjustable sliders and break-even analysis
- Design approach follows Gestalt principles and Cole Nussbaumer Knaflic's storytelling framework: left-aligned takeaway titles, neutral gray axes, single accent color, direct labeling over legends, and annotated benchmark lines

## Ethical Considerations
The employer-sites dataset is synthetic and clearly labeled as such across all materials. Sensitivity views show ranges rather than single numbers to avoid overstating precision. County burden figures are derived directly from the National Database of Childcare Prices with light cleaning only (data type fixes and duplicate removal). All filter scopes (CA and WA hubs, top employer lists) are stated explicitly in each slide or figure.

## Repository Contents
```
childcare-stipend-roi/
├── childcare_data_exploration.ipynb      # Initial data health checks and exploratory analysis
├── childcare_burden_analysis.ipynb       # Full analysis: burden calculations, visualizations, ROI modeling
├── Project_writeup.pdf                   # Final project write-up
├── PowerPoint_Presentation.pdf           # Slide deck
├── Executive_Brief.pdf                   # One-page executive summary
├── ROI_Dashboard.pbix                    # Power BI dashboard (interactive)
├── ROI_Dashboard.pdf                     # Dashboard export
├── nationaldatabaseofchildcareprices.xlsx
├── employer_sites_hr_synthetic.csv
├── hub_stipend_needed_to_7pct.csv
├── slide2_state_burden_table.csv
├── Codes.xlsx
└── README.md
```

## How to Run
1. Install dependencies: `pip install pandas numpy matplotlib openpyxl`
2. Run `childcare_data_exploration.ipynb` first for initial data review
3. Run `childcare_burden_analysis.ipynb` for the full analysis and visualizations
4. Open `ROI_Dashboard.pbix` in Power BI Desktop to interact with the ROI calculator

  
---
  
*Part of my [Data Science Portfolio](https://github.com/nananmorgan/data-science-portfolio)*
  
---
