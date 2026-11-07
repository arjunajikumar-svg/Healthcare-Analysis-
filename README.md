# Healthcare Analysis (Excel)

An Excel-based analysis of **2,335 patient records** that joins medical examination, hospitalisation and customer data into one cleaned dataset, then uses pivot charts and a dashboard to see what drives hospital charges.

## Objective
Clean three raw healthcare tables, combine them, and answer: which patient and hospital factors (smoking, weight status, diabetes status, age, hospital tier) are linked to higher treatment charges?

## Dataset
- File: `Healthcare.xlsx`
- Records: 2,335 customers (patient names are kept out of this README and should be removed or anonymised before the workbook is shared publicly)
- Source sheets: `Customer Names`, `Medical Examinations`, `Hospitalisation Details`
- Combined sheet (`HealtCare`): 17 fields, including BMI, HbA1c, Weight Status, Diabetic Status, Heart Issues, Any Transplants, Cancer history, Number of Major Surgeries, Smoker, Date of Birth, Age, Charges, Hospital tier, City tier and State ID

## Excel Skills Used
- **Data cleaning, Phase 1 (missing values):** `COUNTIF` to count blanks, `IF` + `ISBLANK` + `AVERAGE` to fill numeric gaps (e.g. average for the missing year), most frequent value for categories (Hospital tier, City tier, Smoker), and "Sep" as the default for missing months
- **Data cleaning, Phase 2 (formatting and consistency):** Text to Columns, Find & Replace to fix inconsistent labels, `IFS` for grouping logic, `DATEVALUE` to merge year, month and date into a real date, `DATEDIF` to calculate exact age
- Merging three sheets into one analysis table
- Pivot Tables and Pivot Charts (doughnut, bar and line) on dedicated sheets
- A final `Dashboard` sheet with 6 charts

## Key Insights
Figures below are averages calculated from the combined `HealtCare` sheet.
- **Smoking is the biggest cost driver:** smokers average about 32,900 in charges versus about 8,400 for non-smokers (roughly 3.9x). Smokers are 488 of 2,335 patients (about 21%).
- **Hospital tier matters:** Tier 1 hospitals average about 30,100 per patient, against about 11,900 for Tier 2 and about 9,500 for Tier 3.
- **Weight status:** patients with obesity (the largest group, 1,221 patients) average about 16,700, compared with about 9,800 for normal weight and about 6,900 for underweight.
- **Diabetes:** diabetic patients average about 16,100 versus about 12,100 for patients with normal status.
- **Age:** average charges rise steadily from about 8,500 (age 25 and under) to about 18,400 (age 55 and over).
- **Cancer history and heart issues** showed little difference in average charges in this dataset.

## Preview
<img width="1278" height="590" alt="Screenshot 2026-11-07 151723" src="https://github.com/user-attachments/assets/c21b07b2-4c30-4db4-9f6b-c91ba7e08478" />


