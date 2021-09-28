# DAX-Formulas
Here is some of DAX formulas I wrote within Power BI to solve simple up to very advanced analytical problems.

- 1.Totals:
Summary = 
VAR tableGrouped=
    SUMMARIZE('US Superstore data',
              'US Superstore data'[Sub-Category],
              "Total Sales by Sub Category",SUM('US Superstore data'[Sales])
    )
RETURN tableGrouped
