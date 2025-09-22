# Copilot Instructions for Forest-value Project

## Project Overview
- This project estimates the value of forest and agricultural land for Company X, integrating financial, market, and qualitative data.
- Main workflows involve data cleaning, analysis, and visualization using Python (Pandas, NumPy), SQL, and Power BI.
- Data sources are stored in `Data_Sources/` and `Hindamine/` directories, including Excel, CSV, XML, and JSON files.

## Key Files & Directories
- `Forest_value_final.ipynb`, `Forest_value.ipynb`: Main analysis notebooks. Use these for core data processing and modeling.
- `Data_Sources/`: Contains raw data files (Excel, JSON, mapping tables).
- `Hindamine/`: Contains valuation-related data, including subfolders for property and management plan data.
- `README.md`: Project background, business glossary, and data dictionary.

## Data Flow & Patterns
- Data is loaded from Excel/CSV/XML/JSON files, cleaned, and merged using Pandas.
- Mapping tables (e.g., `Tree_Name_mapping.xlsx`) are used for data normalization.
- Calculations for valuation (timber harvest costs, future value, market prices) are performed in notebooks.
- Results are visualized in Power BI (external to repo).

## Developer Workflows
- **No build system or test suite detected.**
- Use Jupyter notebooks for iterative analysis and debugging.
- Version control via Git; feature branches (e.g., `feature/Merge-uuendused`) are used for updates.
- Data protection and quality control are described in the README, but not enforced by code.

## Project-Specific Conventions
- Keep all raw data in `Data_Sources/` and `Hindamine/`.
- Use mapping tables for normalization before analysis.
- Document new analysis steps in the main notebooks.
- Prefer Pandas for all data manipulation; avoid custom parsing unless necessary.

## Integration Points
- External visualization in Power BI (not included in repo).
- No direct API or service integration detected.

## Example: Loading and Merging Data
```python
import pandas as pd
raw = pd.read_excel('Data_Sources/h24.xlsx')
mapping = pd.read_excel('Data_Sources/Tree_Name_mapping.xlsx')
merged = raw.merge(mapping, on='TreeName', how='left')
```

## Guidance for AI Agents
- Focus on notebook-based workflows and Pandas data manipulation.
- Reference mapping tables for normalization.
- Keep new data files organized in the appropriate directory.
- Document any new analysis or workflow steps in the notebooks.
- If adding new data sources, update the README data dictionary.
