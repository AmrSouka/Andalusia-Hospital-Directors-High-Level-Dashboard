# Andalusia Hospital — Directors High-Level Dashboard

A Power BI dashboard built for Andalusia Hospital's leadership team, giving directors a single view of clinical revenue, volume, and cost performance across departments and business units.

![Dashboard Overview](docs/images/dashboard-overview.png)

## Overview

The **Directors High Level Dashboard** consolidates hospital-wide performance into one page, tracking Revenue, Volume, and Cost per Visit (CPV) against baseline and target figures, with drill-down into individual departments and business units.

## Filters

| Filter | Options |
|---|---|
| Country | All / by country |
| Business Unit | All / by unit |
| Month | All / by month |
| Payment Type | Cash / Credit |

## Key Metrics (Top KPI Cards)

| Metric | Baseline | Historical | Actual | Target | Ach% | G% |
|---|---|---|---|---|---|---|
| Total Revenue | $695M | $445M | $552M | $725M | 76% | -21% |
| OPD Volume | 240K | 176K | 172K | 244K | 71% | -28% |
| Total CPV | $4.44M | $3.28M | $4.06M | $4.52M | 90% | -8.5% |

- **Ach%** — Actual achievement against target
- **G%** — Growth/variance versus baseline

## Unified Medical Department Table

A detailed breakdown by department (Cath LAB, CCU, ER, External – Pharmacy Sales, ICU, Inpatient, and more), each showing:

- Baseline / Historical / Actual / Target Revenue
- Achievement % and Growth %
- Baseline / Historical / Actual / Target Volume

## Business Unit Scorecards

Dedicated Revenue, Volume, and RPP/CPV cards for individual business units, including:

- **Digital Marketing** — Revenue, Volume, RPP (Revenue Per Patient)
- **Medical CRM** — Revenue, Volume, CPV

Each scorecard follows the same Baseline / Actual / Target / Ach% / G% structure used at the top level, so directors can compare unit-level performance against the hospital-wide picture.

## Tech Stack

- **Power BI Desktop** — data modeling, DAX measures, and report layout
- Data sources: hospital revenue, volume, and cost datasets (connected via Power BI's `Get data`)

## Repository Structure

```
andalusia-hospital-dashboard/
├── README.md
├── LICENSE
├── .gitignore
├── docs/
│   ├── images/
│   │   └── dashboard-overview.png
│   └── CHANGELOG.md
└── pbix/
    └── (place your .pbix file here)
```

## Getting Started

1. Clone this repository.
2. Open the `.pbix` file (once added under `pbix/`) in Power BI Desktop.
3. Update data source connections under **Home > Transform data > Data source settings**.
4. Refresh the data model.

## Roadmap / Ideas

- [ ] Add per-department drill-through pages
- [ ] Add trend charts (Actual vs Target over time)
- [ ] Add mobile-optimized layout
- [ ] Document DAX measures in `docs/dax-reference.md`

## License

See [LICENSE](LICENSE).
