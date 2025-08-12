# Bill Generator

A Streamlit app and CLI to generate A4 documents (PDF, DOCX) with uniform 10 mm margins from an Excel input, plus a separate set of LaTeX PDFs.

## Features
- HTML -> PDF (A4, 10 mm margins) via wkhtmltopdf
- DOCX (A4, 10 mm margins)
- LaTeX templates compiled to PDFs into `latex_pdfs/`
- Merged PDF of all pages
- ZIP bundle of all outputs

## Prerequisites
- Python 3.10+
- wkhtmltopdf (for HTML PDFs) — optional; app will still run without it
- TeX Live (for LaTeX PDFs) — optional

On Debian/Ubuntu:
```bash
sudo apt-get update -y
sudo apt-get install -y python3-venv
# Optional but recommended for full output set
sudo apt-get install -y texlive-latex-base texlive-latex-recommended texlive-fonts-recommended
# wkhtmltopdf installation varies by distro. Use your package manager or download a static build.
```

## Setup
```bash
git clone <your-repo-url>
cd <repo>
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Run the UI (Streamlit)
```bash
source .venv/bin/activate
streamlit run streamlit_app.py
```
Then upload your `.xlsx`, set premium settings, and download the ZIP.

## Run programmatically (CLI)
```bash
source .venv/bin/activate
python streamlit_app.py INPUT.xlsx --premium-percent 2.5 --premium-type add --out ./output
```
- `--premium-type`: `add` or `deduct`
- Outputs will be written in `--out` directory with a `bill_output.zip` containing:
  - `BILL_AND_DEVIATION.pdf` (merged)
  - Individual PDFs per page
  - DOCX per page
  - `latex_pdfs/` with LaTeX-generated PDFs

## Logo
The app auto-loads a logo from the GitHub repo `CRAJKUMARSINGH/Priyanka_TenderV01` if available.

## Notes
- If wkhtmltopdf is missing, HTML->PDF is skipped with a warning.
- LaTeX compilation requires `pdflatex`; if missing, LaTeX PDFs are skipped with a warning.
