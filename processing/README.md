# Processing

This folder contains scripts used to transform raw match JSON files into a structured dataset.

## Files

- `json_to_df.py` - Converts JSON match data to CSV format

### json_to_df.py

This script:
- Reads multiple JSON files from the input directory
- Extracts nested match and ball-by-ball data
- Combines data into a single pandas DataFrame
- Outputs a clean CSV dataset for analysis
