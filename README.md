# INTERNSHIP PROJECTS

Practical machine learning portfolio with projects in sales forecasting, NLP ticket classification, and resume screening.

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-f7931e)
![NLP](https://img.shields.io/badge/NLP-Text%20Analytics-0f766e)
![Forecasting](https://img.shields.io/badge/Focus-Business%20Forecasting-1d4ed8)
![Status](https://img.shields.io/badge/Portfolio-Active-16a34a)

This repository showcases three practical machine learning projects built around real business operations, not toy chatbots. Each project solves a different decision-support problem: demand forecasting, support ticket routing, and candidate screening.

## About Me

I am building a portfolio focused on practical machine learning systems that solve real business problems. My work here emphasizes clear problem framing, clean Python implementation, interpretable results, and project write-ups that both technical and non-technical stakeholders can understand.

This portfolio is especially focused on:

- machine learning for business operations
- NLP workflows for support and hiring decisions
- decision-support systems that can be explained clearly to managers, recruiters, and clients

## Portfolio Highlights

| Project | Business Use Case | Core ML/NLP Approach | Current Result |
| --- | --- | --- | --- |
| `superstore-sales-forecasting` | Forecast sales for planning and inventory | Time-series style feature engineering with `Ridge` regression | 6-month forecast with holdout evaluation and charts |
| `support-ticket-classification` | Route customer tickets and surface urgency | TF-IDF plus linear text classification | `75.0%` category accuracy on sample labeled tickets |
| `resume-screening-system` | Rank candidates against a target role | TF-IDF similarity plus skill coverage scoring | Top candidate identified with explicit skill gaps |

## Why This Repo Stands Out

- Focuses on business workflows that companies actually automate
- Includes runnable code, sample data, generated outputs, and project-level documentation
- Balances technical implementation with plain-language explanations for managers and recruiters

## Repository Structure

```text
FUTURE INTERN PROJECTS/
  projects/
    superstore-sales-forecasting/
    support-ticket-classification/
    resume-screening-system/
```

## Included Projects

### 1. Superstore Sales Forecasting

This project was migrated from the earlier standalone `superstore-sales-forecasting` repository so it can live alongside the rest of your portfolio.

- Path: `projects/superstore-sales-forecasting`
- Main script: `python src/forecast_sales.py`
- Business value: supports forecasting, stock planning, and budget preparation
- Key output: `outputs/forecast_dashboard.png`

### 2. Support Ticket Classification and Prioritization

This NLP workflow reads support tickets, cleans text, converts it into TF-IDF features, predicts the ticket category, and predicts whether the issue is high, medium, or low priority.

- Path: `projects/support-ticket-classification`
- Main script: `python src/train_ticket_models.py`
- Business value: helps support teams route tickets faster and focus on urgent issues first
- Key output: `outputs/category_confusion_matrix.png`

### 3. Resume and Candidate Screening System

This project ranks resumes against a target job description using TF-IDF similarity plus skill coverage analysis. It also shows which required skills are missing for each candidate.

- Path: `projects/resume-screening-system`
- Main script: `python src/rank_resumes.py`
- Business value: helps recruiters shortlist faster and explain candidate fit more clearly
- Key output: `outputs/candidate_rankings.png`

## Quick Results

### Superstore Sales Forecasting

- Forecasted next 6 months total: `$340,964`
- Highest forecast month: `March 2019`
- Visuals: `forecast_dashboard.png` and `sales_forecast_outlook.png`

### Support Ticket Classification

- Category accuracy: `75.0%`
- Priority accuracy: `41.7%`
- Best use today: first-pass routing, with more labeled priority data recommended for production

### Resume Screening System

- Candidates screened: `5`
- Top-ranked candidate: `Emma Jacobs`
- Key gap for top candidate: `machine learning`, `scikit-learn`

## Setup

Create a virtual environment and install the shared dependencies:

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

## Run Each Project

```bash
cd projects/superstore-sales-forecasting
python src/forecast_sales.py

cd ..\support-ticket-classification
python src/train_ticket_models.py

cd ..\resume-screening-system
python src/rank_resumes.py
```

## Notes

- The support ticket and resume projects include sample datasets so the code runs out of the box.
- Both new projects are structured so you can replace the sample data with Kaggle datasets later without changing the pipeline design.
- The repository is already connected to GitHub and ready for future updates from `main`.
