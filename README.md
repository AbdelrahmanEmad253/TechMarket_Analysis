# TechMarket Analysis: what the tech job market asks for

A team project from the **NTI** technical track: job data from **7 global platforms** (TechLayoff, Upwork, Indeed, Wuzzuf, Egytech, Monster, RemoteOK), cleaned in Excel, modelled and visualised in Power BI, plus a skills-based job recommender. The project post reports 600,000+ job records in total; this repo holds the scrapers, cleaned data and dashboards we shared.

> Business question: *which roles and skills are in demand, where, and for what seniority?* The goal is to help job seekers decide what to learn and how to position themselves.

## Pipeline

```
scraping/  ->  cleaned_data/  ->  PowerBI/                       ->  wuzzuf Jobs recommendation system/
scrapers       cleaned in Excel   galaxy schema (7 fact tables,      Streamlit app: enter skills +
(Python)                          18 dimensions), dashboards          location, get matching jobs
```

## What's inside

| Folder | Contents |
|---|---|
| `scraping/` | Scrapers in this repo: EgyTech, RemoteOK, Wuzzuf |
| `cleaned_data/` | Cleaned datasets |
| `PowerBI/` | Power BI dashboards (galaxy-schema model) |
| `wuzzuf Jobs recommendation system/` | Content-based recommender (TF-IDF + cosine similarity) with a Streamlit UI |
| `Final_project_NTI_powerpoint.pptx` | Final presentation |

## What the dashboards cover

- Global tech salaries and layoffs
- Country deep dives (Egypt, USA)
- Skill demand by job title (50+ titles) and experience level
- Which companies and regions are hiring, by job type and seniority

## Stack

Python (requests, BeautifulSoup, Selenium, pandas), Excel, Power BI, scikit-learn (TF-IDF, cosine similarity), Streamlit

## My role

Team of two with **Ali Ahmed Sherif**, under the mentorship of **Eng. Huda Hemdan** at the National Telecommunication Institute (NTI). The data collection, cleaning and Power BI modelling were joint work; Ali built the recommendation engine.
