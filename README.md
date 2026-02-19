# AI Assistant Impact Report (Quarto Demo)

This repository contains a **demonstration analytical report** built with [Quarto](https://quarto.org) that illustrates how the impact of an AI assistant on data work, productivity, and delivery speed can be measured and communicated.

The report is designed as an **example for a POSIT Conference 2026 talk**. It focuses on *storytelling with metrics*, executive-ready visualizations, and how AI-assisted analytics reshapes the role of Data Science inside organizations.

All data used in the report is **synthetic** and created solely for illustrative purposes.

## What This Report Demonstrates

The report shows how to:

* Quantify the impact of an AI assistant beyond simple adoption metrics
* Connect self-service analytics to delivery throughput and productivity
* Visualize structural changes in Data Science work
* Combine narrative, metrics, and design using Quarto

Key themes include:

* Reduction in ad-hoc data requests
* Compression of time-to-insight
* Faster project delivery
* Shifts in how Data Science teams spend their time

## Repository Structure

```
.
├── ai_assistant_report.qmd   # Main Quarto report
├── footer.html               # Custom HTML footer
├── report_style.css          # Report-specific styling
└── README.md
```

### `ai_assistant_report.qmd`

The main Quarto document. It includes:

* An executive summary with key metrics
* Multiple analytical sections with ggplot2 visualizations
* Narrative explanations focused on productivity and delivery
* Custom layout using Quarto sections, columns, and cards

The report is rendered as **HTML** and uses Quarto’s layout system without custom grids.

### `footer.html`

A lightweight HTML footer injected at render time that:

* Clarifies the report is a demonstration example
* References its use in a POSIT Conference 2026 talk
* Provides author attribution

The footer is included via `include-after-body` in the Quarto configuration.

### `report_style.css`

Custom CSS used to:

* Apply consistent typography and spacing
* Style highlighted sections and metric blocks
* Preserve Quarto’s underlying layout and grid system
* Support a clean, executive-friendly visual style

## How to Render the Report

### Requirements

* **R** (≥ 4.2 recommended)
* **Quarto** (≥ 1.4)
* R packages used in the report:

  * `tidyverse`
  * `ggalluvial`
  * `patchwork`

Install required packages if needed:

```r
install.packages(c(
  "tidyverse",
  "ggalluvial",
  "patchwork"
))
```

### Render the Report

From the repository root:

```bash
quarto render ai_assistant_report.qmd
```

This will generate an HTML report using the provided CSS and footer.

## Notes on Scope and Intent

* This report is **not** a benchmark, product evaluation, or real company case study
* Metrics, trends, and distributions are **synthetic**
* The purpose is to demonstrate **how to structure and communicate impact**, not to validate a specific tool or implementation

## Attribution

Prepared as a demonstration example for a **POSIT Conference 2026** talk.
© 2026 Paula LC
