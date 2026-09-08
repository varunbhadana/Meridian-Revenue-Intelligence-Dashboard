# Meridian Goods — Sales Intelligence Report

An interactive sales performance dashboard built as a BI-style report canvas: KPI tiles, trend and category charts, a regional heatmap, and a target-achievement gauge — all filter-driven and calculated live in the browser.

**Live demo:** https://varunbhadana.github.io/meridian-sales-dashboard/

![Status](https://img.shields.io/badge/status-live-brightgreen) ![Type](https://img.shields.io/badge/type-interactive%20dashboard-blue)

## Overview

This project simulates a two-year sales dataset (FY24–FY25) for a fictional multi-region retailer and presents it through a report-canvas layout inspired by enterprise BI tools. Every visual — KPI cards, charts, table, heatmap — responds instantly to the filter pane, with no page reloads and no backend.

## Features

- **KPI strip** — total revenue, gross profit, units sold, average order value, and year-over-year growth, recalculated on every filter change
- **Filter pane** — fiscal year (radio), region and category (checkboxes), all cross-filtering the entire report
- **Revenue trend** — monthly line chart with an automatic seasonal-peak annotation
- **Revenue mix** — category breakdown donut chart
- **Revenue by region** — ranked horizontal bar chart
- **Target achievement** — gauge comparing filtered revenue against a modeled target
- **Revenue heatmap** — region × month intensity grid
- **Top products** — ranked list with inline share bars and YoY growth

## Tech stack

- HTML, CSS, vanilla JavaScript (no build step)
- [Chart.js](https://www.chartjs.org/) for charts
- Google Fonts (Inter, Fraunces)
- A seeded pseudo-random generator produces a reproducible sample dataset directly in the browser — no external data file needed

## Running locally

Clone the repo and open `index.html` in any browser — no installation or server required.

```bash
git clone https://github.com/varunbhadana/meridian-sales-dashboard.git
cd meridian-sales-dashboard
open index.html   # or just double-click the file
```

## Data note

All figures are generated sample data for demonstration purposes and do not represent real transactions.

## Author

Built by [Varun Bhadana](https://github.com/varunbhadana).
