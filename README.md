# Business Analytics Job Ready Project

Which employees are likely to attrit?

**Stakeholder:** People Analytics Partner

## Key Insights

- Overtime above 15 hours/month increases attrition probability.
- Two manager changes in a year is a strong attrition signal.
- Engagement scores below 55 precede departures within two quarters.

## Dataset

Primary file: `data/employee_attrition.csv`  
Target variable: `left_company`

## Getting Started

```bash
pip install -r requirements.txt
jupyter notebook notebooks/analysis.ipynb
```


## Next Steps

**Done.** Weekly stakeholder report automation is implemented — see ### Implemented below.

---
*Analytics portfolio project — 2025-08*

### Implemented

```bash
pip install -r requirements.txt
python scripts/weekly_report.py
```