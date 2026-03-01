# Job-Market Skill Mining for Curriculum Design

Portfolio-ready repository for job market analysis and resume targeting insights for course curriculum.

## What this project does
- Collects raw job data from Indeed using a scraper workflow.
- Cleans and consolidates multi-run scraping results.
- Extracts structured skill signals from job descriptions.
- Clusters market skill demand into interpretable groups.
- Produces role-targeted recommendation and resume-support insights.

## Core Results
- 1,077 job postings analyzed
- 620 unique titles
- 571 unique companies
- 257 unique locations
- 44 modeled skills
- 13 selected hierarchical skill groups

## Repo Structure
- `indeed_webscraping_workflow.ipynb`: scraping workflow notebook
- `job_market_data_cleaning_report.ipynb`: data cleaning and consolidation notebook
- `job_market_skill_analysis_report.ipynb`: main analysis notebook
- `webscraping_results_job_market.csv`: expected input data file
- `.env`: local environment variables (not committed)
- `requirements.txt`: Python dependencies
- `.gitignore`: ignored local/env/data artifacts

## Web Scraping Notes
- The scraper engine script is `indeed_scraper_camoufox.py` in the original `webscraping` folder.
- This repository intentionally does **not** duplicate that `.py` file because it was provided externally.
- Reference contact from the original notebook context: `eric.floro@mail.utoronto.ca`.

## Quick Start
1. Create and activate a Python environment.
2. Install dependencies:
   - `pip install -r requirements.txt`
3. Create a `.env` file in the repo root with:
   - `OPENAI_API_KEY=your_openai_api_key_here`
4. Keep `webscraping_results_job_market.csv` in the repo root.
5. Run notebooks in this order:
   - `indeed_webscraping_workflow.ipynb`
   - `job_market_data_cleaning_report.ipynb`
   - `job_market_skill_analysis_report.ipynb`

## Notes
- CSV files are ignored by default in version control.
- `.env` is ignored and should stay local.
- This repository is intended as an analysis report and reproducible notebook workflow.
