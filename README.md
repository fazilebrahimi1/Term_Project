# Does Higher Internet Penetration Cause Lower Unemployment?
### DA4: Causality — Term Project | Central European University | April 2025
**Author:** Fazile Brahimi

## Research Question
Does higher internet penetration causally reduce unemployment rates across countries?

## Main Finding
After controlling for country and year fixed effects, internet penetration has no 
statistically significant average effect on unemployment (coef = -0.0016, se = 0.0080, 
p = 0.845). However, the effect is nearly four times larger in high-income countries 
(-0.039) than in low/middle-income countries (-0.010), consistent with the 
complementarity hypothesis.

## Repository Contents
- `analysis.ipynb` — Full analysis notebook (data loading, cleaning, regressions, figures)
- `main_figure.png` — Figure 1: Internet penetration vs unemployment (scatter + time trends)
- `heterogeneity_figure.png` — Figure 2: Heterogeneity by income group
- `Term_Project.pdf` — Final paper
- `requirements.txt` — Python dependencies

## Data
Raw data downloaded from World Bank Open Data (no login required):
- **Y:** Unemployment rate (% of labor force) — https://data.worldbank.org/indicator/SL.UEM.TOTL.ZS
- **X:** Internet users (% of population) — https://data.worldbank.org/indicator/IT.NET.USER.ZS

Download both as CSV, place in the same folder as `analysis.ipynb`, and update 
the filenames in Cell 1 of the notebook.

## How to Reproduce
1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Download the two World Bank CSVs (links above)
4. Run `analysis.ipynb` cell by cell

## Reference
Atasoy, H. (2013). The effects of broadband internet expansion on labor market outcomes. 
ILR Review, 66(2), 315–345. https://ssrn.com/abstract=1890709
