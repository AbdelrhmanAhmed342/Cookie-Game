```markdown
# Cookie Cats A/B Testing & Retention Prediction

[![GitHub Repo stars](https://img.shields.io/github/stars/AbdelrhmanAhmed342/cookie-cats-ab-testing?style=social)](https://github.com/AbdelrhmanAhmed342/cookie-cats-ab-testing)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.7+](https://img.shields.io/badge/Python-3.7%2B-blue.svg)](https://www.python.org/downloads/)

## Project Overview

End-to-end data science project analyzing the famous **Cookie Cats** mobile game A/B test.  
We test whether moving the first paywall from level 30 → 40 affects player retention, then build a machine learning model to predict 7-day retention.

**Key Findings**  
- A/B test: gate_40 causes a statistically significant ~4.3% relative drop in 7-day retention (p=0.0016)  
- ML model (Random Forest): ROC-AUC = **0.885**, recall on retained players = **79–81%**  
- Feature importance:  
  - `sum_gamerounds` → **81.9%**  
  - `retention_1` → **18.1%**  
  - `version` (gate position) → **only 0.06%**  

**Business takeaway**: Early engagement completely dominates retention — gate position barely matters.

## Dataset

Source: [Mobile Games A/B Testing - Cookie Cats](https://www.kaggle.com/datasets/mursideyarkin/mobile-games-ab-testing-cookie-cats)  
90,189 players • 5 columns • Perfectly balanced A/B split

## Tech Stack

- Python (pandas, numpy, matplotlib, seaborn, scipy, scikit-learn)  
- Google Colab notebook  
- Power BI dashboard (optional)

## Repo Structure

```
cookie-cats-ab-testing/
├── README.md
├── cookie_cats.csv
├── Cookie_Cats_Analysis.ipynb          # Full EDA + A/B + ML
├── powerbi_dashboard.pbix              # Interactive dashboard (optional)
├── outputs/                            # Plots & predictions
└── LICENSE
```

## How to Run

```bash
git clone https://github.com/AbdelrhmanAhmed342/cookie-cats-ab-testing.git
cd cookie-cats-ab-testing
# Open Cookie_Cats_Analysis.ipynb in Colab or Jupyter
```

Just run all cells — everything works out of the box.

## Key Results

- 7-day retention: gate_30 = 19.0% vs gate_40 = 18.2%  
- Random Forest feature importance proves early playtime is king  
- Model can predict day-7 retention as early as day 2–3

## Author

**Abdelrhman Ahmed**  
**Abdelrhman Ahmed**  
GitHub: [@AbdelrhmanAhmed342](https://github.com/AbdelrhmanAhmed342)  
LinkedIn: [linkedin.com/in/abdelrhman-ahmed-342](https://www.linkedin.com/in/abdelrhman-ahmed-342)  
Portfolio: [abdelrhmanahmed342.github.io]([https://abdelrhmanahmed342.github.io](https://abdelrhmanahmed342.github.io/Abdelrahman_Portfolio/))  
Email: abdo.elgoneeemy@gmail.com

Built with passion for data science. Star if you like it!

---
MIT License • Free to use, modify, and share
