# DFI Transaction Dashboard

An interactive browser-based dashboard for exploring DFI (Development Finance Institution) private investment transactions across 14 institutions: IFC, BII, DFC, IDB Invest, Proparco, FMO, Norfund, Finnfund, BIO, SIFEM, FinDev Canada, Swedfund, DEG, and IFU.

## Features

- **Full-text search** across client names, project names, and countries
- **Searchable multi-select filters** for DFI, region, country, sector, status, and investment type
- **Amount and year range filters**
- **Table view** — sortable, paginated, with links to original project pages
- **Map view** — proportional circle markers per country, coloured by region, with click-to-filter
- **Summary stats** — live transaction count, total committed capital, countries, DFIs, unique clients

## Data

The dataset covers ~15,900 transactions across 14 DFIs with standardised taxonomy fields for region, sector, status, and investment type.

## Setup

### Local

Just open `index.html` in a browser — no build step needed. Make sure `data/DFI_Unified_Dataset.csv` is present.

> **Note:** Most browsers block local file fetches. Use a simple local server instead:
> ```bash
> # Python 3
> python -m http.server 8000
> # then open http://localhost:8000
> ```

### GitHub Pages

1. Push this folder (with `data/DFI_Unified_Dataset.csv`) to a GitHub repository
2. Go to **Settings → Pages → Source → main branch / root**
3. The dashboard will be live at `https://<username>.github.io/<repo>/`

## File structure

```
├── index.html                  # Dashboard (self-contained, CDN dependencies)
├── data/
│   └── DFI_Unified_Dataset.csv # Dataset (~7.5 MB)
└── README.md
```

## Sources

EDFI members (BII, BIO, DEG, FMO, Finnfund, IFU, Norfund, Proparco, SIFEM), IFC, IDB Invest, DFC, FinDev Canada.
