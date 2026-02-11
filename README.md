# AI Workforce Intelligence: Strategic EDA (2010-2025)

![Market Header](https://img.shields.io/badge/Status-Executive_Ready-success)
![Tools](https://img.shields.io/badge/Tools-uv_|_Pandas_|_Plotly-blue)
![Language](https://img.shields.io/badge/Language-English-orange)

## Overview
This repository contains a high-velocity Exploratory Data Analysis (EDA) of the global AI job market transition from 2010 to 2025. This project was developed to provide a CEO-level overview of the **Economic ROI of AI Skills** and the **Structural Risks of Automation** across different global regions.

---

## Where to Look
* Full Analysis Notebook: notebooks/01_eda_ai_jobs.ipynb
* Executive Summary: reports/EXECUTIVE_REPORT.md
* High-Resolution Figures: reports/figures/

---

## EDA Workflow

The analysis followed a structured exploratory pipeline:

1. Data loading and schema inspection (`info`, `describe`)
2. Missing value analysis (null % distribution)
3. Nested Grouped IQR filtering (by region + seniority level)
4. Feature engineering (AI intensity, risk segmentation)
5. Univariate analysis (distribution & outliers)
6. Bivariate analysis (correlation & grouped comparison)
7. Executive insight extraction

---

## Quick Start (For Evaluators)

This project utilizes **`uv`**, the high-performance Rust-based Python package manager, to ensure ultra-fast and reliable dependency resolution.

### 1. Environment Setup
```bash
# Sync environment and install all dependencies from uv.lock
uv sync

# Activate the virtual environment
source .venv/bin/activate
```

#### Alternative Setup (Standard pip)

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

### 2. Running the Analysis
The core analytical engine is located in:
notebooks/01_eda_ai_jobs.ipynb

---

## The Analytical Storyline (The 5-Graph Journey)
To provide actionable intelligence, the analysis follows a sequential narrative:
1. The Baseline: Establishing the global salary standard using Nested Grouped IQR to remove geographic and seniority noise.
2. The Locality Paradox: Visualizing why a North American Intern often out-earns a South Asian Senior, identifying talent arbitrage opportunities.
3. The AI Multiplier: Proving the linear correlation between AI technical intensity and professional compensation.
4. The Automation Trap: Identifying roles driving at full speed toward a "Mechanical Failure" (Displacement risk > 0.7).
5. Strategic Resilience: Mapping industry-level investment priorities for workforce reskilling.


### Why Nested Grouped IQR?

Salary distributions differ significantly across regions and seniority levels.
Applying a global IQR would remove legitimate high-income roles in mature markets.

To avoid geographic bias, outliers were filtered within each (region, seniority) group.
This ensures that extreme values are evaluated relative to comparable peers.

### Outlier Filtering Details:
* Nested Grouped IQR applied within (region, seniority)
* Removed 6.5% of total observations
* Post-filter dataset size: n = 4,680


---

## Branching Strategy
This project follows a strict task-based branching model to maintain code integrity and auditability:
* `task/1-data-preprocessing`: Cleaning, Null handling, and Nested IQR filtering.
* `task/2-salary-baseline`: Visualizing the mainstream market floor.
* `task/3-value-correlation`: Analyzing the ROI of AI integration levels.
* `task/4-risk-impact`: Mapping automation risk and time-series growth decay.
* `task/5-executive-report`: Finalizing the visual summary and PDF export.

---

## Project Structure
```text
.
├── data
│   ├── raw           # Original dataset
│   └── processed     # Refined data after Nested IQR processing
├── notebooks         # Core analysis and visualizations (.ipynb)
├── reports
│   ├── figures       # High-resolution PNGs for executive viewing
│   └── EXECUTIVE_REPORT.md  # CEO-level strategic summary
├── pyproject.toml    # Project metadata and uv configuration
└── uv.lock           # Cryptographically locked dependency tree
```

---

## Strategic Conclusion
> "The analysis suggests that regional maturity influences baseline salary levels, while AI intensity significantly affects compensation growth. Strategic hiring should therefore consider both geographic structure and AI capability depth."

---

Created by: Mirae Kang | Submission Date: February 10, 2026