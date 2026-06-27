# AI Data Cleaner

A Streamlit desktop app that loads messy accounting datasets and helps clean them for analysis.

<img width="1917" height="879" alt="image" src="https://github.com/user-attachments/assets/db7333e4-a5dd-43bf-889f-30d4fe43fc69" />


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

<img width="1915" height="875" alt="image" src="https://github.com/user-attachments/assets/b9c33078-42ea-48a2-bd24-4e6f5cfbb115" />
  <img width="1909" height="882" alt="image" src="https://github.com/user-attachments/assets/c1949abd-92dc-49fb-8a03-19abccb44762" />
  <img width="1915" height="890" alt="image" src="https://github.com/user-attachments/assets/19527b21-785c-4a7c-b0ed-97ecbaad14ca" />



## About me / connect
I build practical data tools that help finance and accounting teams move from messy exports to analysis-ready datasets.
