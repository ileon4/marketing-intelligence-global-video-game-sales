# Marketing Intelligence Global Video Game Sales Analysis

This project analyzes historical video game sales to identify what factors are associated with market performance across regions and platforms.

## Executive Summary

The analysis finds that global sales peaked between about 2006 and 2011, then declined in later years. Regional preferences are not uniform, especially for Japan compared with North America and Europe, and platform performance changes over time as console generations shift. These patterns support region-specific and time-aware release strategies.

## Project Structure

```text
video-game-sales-analysis/
├── data/
│   ├── games.csv
│   └── raw/
├── images/
├── notebooks/
│   └── Video Game Sales Analysis.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Notebook Organization

The notebook is organized into the following sections:

1. Executive summary and roadmap
2. Environment setup and reproducible path-based data loading
3. Data preparation (types, missing values, derived features)
4. Exploratory analysis (time, platform, genre, and regional patterns)
5. Hypothesis testing
6. Visual export section that saves report figures to `images/`
7. Final conclusion

## Data Source

- Main dataset: `data/games.csv`

## Key Analysis Steps

- Standardized column names and corrected data types
- Reviewed and handled missing values with documented rationale
- Built `total_sales` as a combined sales metric
- Compared platform and genre performance across years and regions
- Tested rating-related hypotheses using two-sample t-tests

## Saved Visualizations

When the export section is run, figures are saved in `images/`:

- `releases_by_year.png`
- `top_platform_total_sales.png`
- `regional_sales_totals.png`

## Setup

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the analysis notebook:

```bash
jupyter notebook notebooks/Video\ Game\ Sales\ Analysis.ipynb
```

## Conclusion

Sales outcomes in this dataset are influenced by both timing and market context. For practical planning, the strongest strategy is to use recent platform-era data and tailor genre/platform mixes by region instead of assuming global uniformity.
