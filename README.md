# AI Workforce Intelligence: Strategic EDA (2010-2025)

![Market Header](https://img.shields.io/badge/Status-Executive_Ready-success)
![Tools](https://img.shields.io/badge/Tools-uv_|_Pandas_|_Plotly-blue)
![Language](https://img.shields.io/badge/Language-English-orange)

## Overview
This repository contains a high-velocity Exploratory Data Analysis (EDA) of the global AI job market transition from 2010 to 2025. This project was developed to provide a CEO-level overview of the **Economic ROI of AI Skills** and the **Structural Risks of Automation** across different global regions.

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
> "In the 2025 AI race, Geography dictates the starting position, but AI Intensity determines the career velocity. Our recommendation is a shift toward AI-augmented hiring in emerging markets."

---

Created by: Mirae Kang
Submission Date: February 10, 2026