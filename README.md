# Conservation Agriculture — Year 4 Survey Portfolio

**Prepared for Winnie K. | Excel analysis, dashboards and M&E reporting**

An aggregate-data case study built from a supplied conservation agriculture monitoring survey. It demonstrates reproducible data validation, descriptive analysis and clear reporting. This is an analytical portfolio, not a causal impact evaluation.

![Portfolio preview](figures/Preview.png)

## Selected results

| Measure | Result | Basis |
|---|---:|---|
| Survey records | 219 | Nonempty submissions |
| Reported CA practice | 95.0% | 208 / 219 |
| All three CA principles, full sample | 73.1% | 160 / 219 |
| Recorded average adequate-food months | 10.37 | 219 valid totals; recall-period caveat |
| Recorded 12-month food adequacy | 58.9% | 129 / 219; recall-period caveat |

## Deliverables

- [Visual case study](reports/Portfolio.pdf)
- [Editable case study](reports/Portfolio.docx)
- [Excel dashboard and aggregate tables](reports/Results.xlsx)
- [Methods and limitations](METHODS.md)
- [Upwork portfolio wording](UPWORK_COPY.md)
- CSV tables in `data/` and PNG charts in `figures/`
- `src/analyze.py`: private-source aggregation
- `src/build_portfolio.py`: charts, workbook, PDF and Word generation from aggregate tables

## Run with the included aggregate data

```bash
python -m venv .venv
# Activate your environment, then:
pip install -r requirements.txt
python src/build_portfolio.py
```

## Rebuild from the original export privately

Place the original workbook outside this repository or in ignored `private/`.

```bash
python src/analyze.py /path/to/CA_YR4_RESULTS.xlsx
python src/build_portfolio.py
```

The importer uses explicit column positions for the supplied schema. Review its mappings before using another survey version. Code for this package was prepared with AI assistance; no prior Python use by the portfolio owner is implied.

## Interpretation and privacy

The source is a single survey export, with no baseline or target table. CA-CF comparisons are descriptive; eligible groups differ and can overlap. Zero harvests on positive areas remain in primary means. Four CF area entries are flagged for review; their values remain unchanged. Food-recall wording is inconsistent, so food indicators are provisional. See METHODS.md for the full rules.

Only aggregate data are included. Do not upload the source workbook, household identifiers, names, GPS coordinates, or open-text responses. No licence is granted over the underlying organisation's data by this package.

## Upload to GitHub

Create a repository named `conservation-agriculture-year4-analysis` and upload the contents of this folder, preserving its directory structure. The ZIP is a transfer package, not the repository itself. Use the description: “Conservation agriculture survey analysis: Excel dashboard, crop yields, food provision and documented data-quality checks.”
