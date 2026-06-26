# Production-Analysis-Dashboard

Project Overview

This project demonstrates professional data organization and analysis for upstream petroleum operations. It showcases how a Production Engineer transforms raw production data into actionable insights through Excel calculations and visualization.

Company: PetroTech Energy Ltd.  
Role: Graduate Production Engineer  
Task: Prepare accurate daily production report  
Date Created**: June 2026


###  Dataset Summary

### Wells Analyzed
- 10 total wells across 3 production fields
- Fields: Alpha, Bravo, Charlie
- Data points**: Oil, Gas, Water, Pressure, Temperature, Operating Status

### Production Range
- Oil Production: 920 - 4,320 bbl/day
- **Total System Production**: 28,430 bbl/day combined
- **Average Production**: 2,843 bbl/day per well

---

## 📑 Workbook Structure

### Sheet 1: Production_Data
Purpose: Raw data repository - single source of truth

Contents:
- 10 production wells with 8 data columns
- **Formatted as Excel Table** for dynamic range references
- Header row frozen for easy scrolling
- Professional formatting with units in column names

Data Format:
| Column | Unit | Range |
|--------|------|-------|
| Oil | bbl/day | 920 - 4,320 |
| Gas | Mscf/day | 160 - 705 |
| Water | bbl/day | 510 - 1,280 |
| Wellhead Pressure | psi | 2,260 - 3,215 |
| Temperature | °F | 171 - 190 |



### Sheet 2: Calculations
Purpose: Derived metrics for engineering analysis

4 Calculated Columns:

#### 1. Total Fluid (bbl/day)
- Formula: Oil + Water
- Why It Matters: Total liquid production tells operators the processing load
- Example: Well A-101: 3,450 + 620 = 4,070 bbl/day total fluid
- Range: 1,430 - 4,830 bbl/day

#### 2. Water Cut (%)
- Formula: (Water ÷ (Oil + Water)) × 100
- Why It Matters: High water content requires expensive separation/disposal
- Interpretation:
  - < 20%: Excellent - minimal water content
  - 20-35%: Monitor - investigate if increasing
  -  > 35%: Investigate - may need workover
- Example: Well C-303: 1,160 ÷ (1,480 + 1,160) = 43.9% (MONITOR)
- Range: 14.7% - 58.1%

#### 3. Gas-Oil Ratio (GOR) (Mscf/bbl)
- Formula: Gas ÷ Oil
- Why It Matters: Indicates wellbore conditions and gas content
- Example: Well B-201: 680 ÷ 4,150 = 0.164 Mscf/bbl
- Range: 0.108 - 0.477 Mscf/bbl

#### 4. Production Category
- High: > 3,500 bbl/day (4 wells)
- Medium: 2,000 - 3,500 bbl/day (4 wells)
- Low: < 2,000 bbl/day (2 wells)
- Why It Matters**: Categorizes wells for targeted management strategies


### Sheet 3: Challenge Questions
Purpose: Demonstrates practical Excel analysis skills

5 Challenge Questions with formulas documented:

| # | Question | Answer | Formula Type |
|---|----------|--------|--------------|
| 1 | Which field produces most oil? | Charlie: 12,330 bbl/day | SUMIF |
| 2 | Highest water cut? | C-303: 43.9% | INDEX/MATCH/MAX |
| 3 | Lowest pressure? | B-203: 2,260 psi | INDEX/MATCH/MIN |
| 4 | Wells needing monitoring? | 2 wells (B-203, C-303) | COUNTIF |
| 5 | Average oil production? | 2,843 bbl/day | AVERAGE |


### Sheet 4: Dashboard
Purpose Executive summary for management review

Key Metrics:
- Total Wells: 10
- Total Oil Production: 28,430 bbl/day
- Average Water Cut: 32.1%
- Wells Monitoring: 2
- Active Wells: 8

Use Case: Morning briefing for Operations Superintendent

### Sheet 5: Notes
Purpose: Reference documentation and formula reference

Contains:
- Formula documentation for all 5 challenge questions
- Answer key with explanations
- Engineering interpretation guidance


##  Engineering Interpretation

### Well Performance Assessment

####  High Performers
- C-304: 4,320 bbl/day (highest producer), Low water cut (10.6%), Active
- B-201: 4,150 bbl/day, Moderate water cut (11.5%), Active
- C-301: 3,890 bbl/day, Moderate water cut (14.1%), Active

#### Wells Requiring Attention
- B-203: 920 bbl/day (lowest production), 58.1% water cut (CRITICAL), Status: Monitor
- C-303: 1,480 bbl/day, 43.9% water cut (HIGH), Status: Monitor
- A-103: 1,820 bbl/day, 34.9% water cut (trending up)

####  Field Comparison
| Field | Total Oil | Avg Water Cut | Wells |
|-------|-----------|---|-------|
| Charlie | 12,330 | 29.6% | 4 |
| Alpha | 8,250 | 33.5% | 3 |
| Bravo | 7,850 | 35.0% | 3 |

Insight: Charlie Field performing best. Bravo Field needs water management focus.


## Excel Skills Demonstrated

### Formulas Used
-  Cell references (absolute and relative)
-  Arithmetic operations (addition, division)
-  Conditional logic (IF statements)
-  Array functions (INDEX, MATCH)
-  Aggregate functions (SUM, AVERAGE, COUNT)
-  Excel Tables (dynamic ranges)

### Formatting Applied
-  Professional header styling
-  Proper number formatting (percentages, decimals)
-  Frozen panes for navigation
-  Column width optimization
- Table formatting for data integrity

## Best Practices Implemented
-  Single source of truth (Production Data sheet)
-  Formulas, not hardcoded values
-  Clear documentation (Notes sheet)
-  Professional presentation
-  Scalable design (easy to add new wells)


Real World Applications

This type of analysis is used daily in upstream operations for:
- Daily production reporting to company leadership
- Well performance monitoring and anomaly detection
- Water management planning (disposal, injection, treatment)
- Maintenance scheduling (wells requiring intervention)
- Economic analysis (identifying underperforming assets)
- Regulatory compliance (daily production tracking for permits)


