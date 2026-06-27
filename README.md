# AI Data Cleaner

A Streamlit desktop app that loads messy accounting datasets and helps clean them for analysis.

![App screenshot](assets/sample_preview.png)

## Why this exists
Financial teams spend too much time fixing inconsistent spreadsheets before they can analyze results. This project makes it easier to turn raw accounting exports into a usable dataset without manual formula work.

## How it works
1. Upload a CSV or Excel file.
2. The app detects issues in the dataset and lets you apply cleaning actions.
3. Use built-in tools to normalize text, remove duplicates, fix dates, and export cleaned data.

## Example output
| Field | Before | After |
|---|---|---|
| `Revenue` | `"$31,990"` | `31990.0` |
| `Date` | `"FY '09"` | `2009-01-01` |
| `Description` | `"  profit & loss statement "` | `"Profit & Loss Statement"` |

## Run locally
```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
streamlit run app/main.py
```

## Tech stack
- Python
- Streamlit
- pandas
- scikit-learn
- openpyxl
- ydata-profiling

## What I'd improve next
- Add a preprocessing step for financial statement-style sheets to infer headers and drop metadata rows.
- Add a column profile page with suggested cleaning actions per field.
- Support more enterprise import formats like fixed-width and XML.

## About me / connect
I build practical data tools that help finance and accounting teams move from messy exports to analysis-ready datasets.
