# Scraping

This folder contains scripts used to collect match-level data from ESPN Cricinfo.

## Files

- `espn_scraper.py`  
    Scrapes scorecard and commentary data for a single match.

- `espn_scraper_loop.py`  
    Iterates through match IDs from an Excel file and runs the scraper across multiple matches.

## Output

Each match is saved as a structured JSON file containing:
- match metadata
- innings data
- ball-by-ball commentary