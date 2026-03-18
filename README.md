# IPL Cricket Analytics Pipeline (2008–2024)

## Overview
This project is an end-to-end cricket analytics pipeline built using publicly available match data from ESPN Cricinfo.

It automates the process of:
- collecting match-level scorecard and commentary data  
- transforming nested JSON into a structured ball-by-ball dataset  
- generating analytical outputs for performance analysis and visualization  

The goal was to replace a manual, time-consuming workflow with a scalable and reproducible system.

---

## Project Evolution

### Phase 1: Manual Workflow (Pre-2022)
Before university, I built an IPL ball-by-ball dataset manually using CSV files from Cricsheet. Each match was added and consolidated into a master dataset, which was then used to build Tableau dashboards.

This phase developed:
- strong understanding of cricket data structures  
- experience with manual data cleaning and consolidation  
- dashboarding and storytelling using Tableau  

🔗 Legacy Tableau Dashboard: https://public.tableau.com/app/profile/sudheesh0807/viz/IPLMAIN/Batters

---

### Phase 2: Automated Pipeline (2025)
This project rebuilds the same workflow using Python to automate the entire pipeline.

Instead of manually updating data, the system:
- scrapes match data directly from ESPN Cricinfo  
- stores raw data in JSON format  
- transforms it into a structured dataset  
- enables scalable analysis and visualization  

---

## Problem Statement
ESPN Cricinfo provides detailed cricket data but does not offer a simple API for large-scale extraction.

Key challenges:
- dynamic page loading  
- commentary data loaded progressively  
- deeply nested JSON structures  

This project solves these challenges by building a scraping and transformation pipeline to generate a clean, analysis-ready dataset covering IPL matches from 2008 to 2024.

---

## Tech Stack
Python · Playwright · Pandas · ujson · Matplotlib · Plotly · Excel · Tableau

---

## Pipeline Workflow
1. Match IDs are stored in an Excel file  
2. Playwright scraper collects scorecard and commentary data  
3. Each match is stored as a JSON file  
4. JSON files are transformed into a single structured dataset  
5. The dataset is used for analysis and visualization  

---

## Dataset Summary
- Matches processed: 1000+  
- Total deliveries: ~3 million  
- Unique players: 800+  
- Venues: 40+  
- Features per delivery: 60+  

---

## Analysis Examples
- Top run scorers across seasons  
- Run rate trends over time  
- Bowling type distribution by over  
- Team scoring patterns by season  
- Wagon wheel analysis for individual players  

---

## Visualizations

### Legacy Dashboard (2022)
Tableau dashboards built on manually compiled data:

- Batting and bowling performance overview  
- Team phase-wise analysis  
- Bowler type breakdown  

See: `tableau/legacy_dashboard/`

---

### Current Analysis (2025)
Python-based visualizations generated from the automated dataset:

- run rate trends  
- batting and bowling patterns  
- situational match analysis  

See: `tableau/current_analysis/`

---

## Repository Structure