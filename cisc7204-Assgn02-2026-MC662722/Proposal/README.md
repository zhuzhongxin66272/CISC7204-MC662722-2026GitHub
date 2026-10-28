# Revised Pair Project Proposal and its materials

Course: CISC7204 Data Science and Data Visualization, Class K, 2026-1, University of Macau
Coursework item: Assignment 02, Revised Project Proposal (pair work)
Pair: Class K Pair 01, Team 02
Members: ZHU ZHONGXIN (MC662722) and DENG YI (MC662921)
Submitted: 25 October 2026

Title: Leisure-Time Physical Activity and the Network Structure of Depressive
Symptoms among U.S. Adults: a NHANES 2017–March 2020 Analysis

## Files

| File | Description |
| --- | --- |
| `CISC7204-Assgn02-Pair01-RevisedProjectProposal.docx` | The proposal document, 5 A4 pages. It is the file submitted at the assignment submission link. |
| `CISC7204-Assgn02-Pair01-ProposalVerification.ipynb` | Executed Jupyter notebook with the full analysis: merging, cleaning, group comparison, adjusted logistic regression, symptom network estimation and the permutation test. |
| `stats_a02.json` | The same results in machine-readable form, written by the last cell of the notebook. |
| `data/DPQ_J.csv`, `data/DEMO_J.csv`, `data/BMX_J.csv`, `data/PAQ_J.csv` | The four NHANES 2017 – March 2020 public-use files used: depression questionnaire, demographics, body measures and physical activity. Converted from the official SAS-XPORT files. |
| `data/NHANES_merged_analysis.csv` | The merged adult table produced by the notebook (5,265 rows). The analysis sample of 4,846 adults with complete values is derived inside the notebook, with the exclusions recorded there. |
| `figures/fig01` to `figures/fig11` | The eleven exploratory figures produced by the notebook. |
| `figures/pf01` to `figures/pf04` | The four composite figures printed in the document. They reuse panels of the exploratory figures at print size. |

## Reproducing the results

Place `data/` next to the notebook and run all cells from top to bottom. The
notebook prints the descriptive results, the group comparisons, the adjusted
models, the network estimates and the permutation test, and writes
`stats_a02.json` at the end. Environment: Anaconda Python 3 with pandas, numpy,
matplotlib, seaborn, scipy, statsmodels and networkx.

## Data source

NHANES 2017 – March 2020 pre-pandemic cycle, National Center for Health
Statistics. Public-use files, no registration required.

- https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?BeginYear=2017
- https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2017/DataFiles/DPQ_J.xpt
- https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2017/DataFiles/DEMO_J.xpt
- https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2017/DataFiles/BMX_J.xpt
- https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2017/DataFiles/PAQ_J.xpt
