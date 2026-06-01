# Exploring Blood Pressure Patterns in the US Adult Population

**Name:** Ani Hovhannisyan

### Description
Analysis of NHANES 2017–2018 data to explore how physical activity, age, gender, 
and income relate to blood pressure and hypertension in US adults.

### Required Libraries
```
pandas
numpy
matplotlib
```
Install with:
```bash
pip install pandas numpy matplotlib
```

### How to Run
1. Download the following four official NHANES 2017–2018 `.xpt` files from the CDC website:
   - [DEMO_J.xpt (Demographics Data)](https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/DEMO_J.xpt)
   - [BPX_J.xpt (Blood Pressure Examination Data)](https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/BPX_J.xpt)
   - [BPQ_J.xpt (Blood Pressure Questionnaire Data)](https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/BPQ_J.xpt)
   - [PAQ_J.xpt (Physical Activity Questionnaire Data)](https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/PAQ_J.xpt)
2. Place all four downloaded `.xpt` files in the exact same folder as your Jupyter notebook.
3. Open `nhanes_bp_analysis.ipynb` in Jupyter.
4. Run all cells from top to bottom (`Kernel → Restart & Run All`).
5. Figures will be automatically saved to the `figures/` folder.


### Three Key Findings
- **Activity and MAP:** Inactive adults have higher mean arterial
pressure than active adults, though distributions overlap 
(median ~90 mmHg), while both the insufficient and active groups show 
lower MAP distributions, suggesting even small amounts of 
physical activity may be associated with lower blood pressure compared to none at all.
- **Age and systolic BP:** Systolic blood pressure increases with age in both sexes, 
however, women experience a steeper rise after age ~55.
- **Income and hypertension:** Hypertension prevalence does not follow a simple
income pattern. The middle income group has the highest rate (~60.0%). That mentioned,
the below poverty group still has the lowest rate (~54.7%). This likely reflects a diagnosis gap: 
lower-income individuals with less healthcare access are less likely to ever be 
formally told they have high blood pressure, causing their true hypertension to 
be undercounted in the data.
