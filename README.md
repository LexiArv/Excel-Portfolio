# Excel Portfolio

Welcome to my Excel Portfolio repository. This repository features business and operational projects designed to solve real world tracking, management, and financial reporting challenges. 

Each project showcases my proficiency in data modeling, logical and financial formulas, conditional formatting, and building robust, automated worksheets.

---

## Projects Overview

### 1. Car Inventory & Fleet Management
* **Location:** `Car_Inventory/Car_Inventory_Example.xlsx`
* **Goal:** Manage a company vehicle fleet, track mileage usage per driver, assess asset age, and automate warranty coverage tracking.

#### ⭐ Actions & Functions Used:
* **Parsing (`LEFT`, `MID`):** Extracted embedded data from the original composite `Car ID` string (using `LEFT` to isolate the 2 letter manufacturer code and `MID` to extract the 2 digit manufacturing year).
* **Relational Data Mapping (`VLOOKUP`):** Used the extracted 2 letter manufacturer code to automatically look up and map the full brand name from a reference master table.
* **String Standardization (`CONCAT`):** Developed a new primary key system by dynamically joining the Make, Model, Color, and unique sequence digits back together into a clean, uniform format.
* **Status Automations (`IF`):** Evaluated whether a vehicle's current mileage falls under its specific warranty threshold to automatically return a status of "Yes" (covered) or "Not Covered".
* **Pivot Tables & Data Summarization:** Constructed a driver mileage breakdown dashboard to track which drivers accumulate the most miles, enabling fleet maintenance forecasting in a dashboard. This enables the operations team to track high mileage accumulation per driver and accurately forecast vehicle maintenance cycles.

---

### 2. Employee Performance & HR Gradebook
* **Location:** `Gradebook/Gradebook_Example.xlsx`
* **Goal:** Track candidate compliance and training metrics across critical testing criteria (Safety, Philosophy, Financial Skills, and Drug Screenings) to automate operational HR decisions.

#### ⭐ Actions & Functions Used:
* **Proportional Percentage Scaling:** Standardized variable testing score ranges by calculating scores using Relative & Absolute Cell References against a fixed master "Points Possible" row.
* **Multi Criteria Evaluation (`IF`, `OR`):** Built the `Fire Employee? True / False` logic gate. The formula flags `True` if an employee fails a zero tolerance compliance test (like the Drug Test) or if their core performance drops below the minimum acceptable business standard.
* **Summary Analytics (`AVERAGE`, `MIN`, `MAX`):** Engineered a baseline performance section at the bottom of the gradebook columns to instantly track cohort averages, isolate lowest scoring parameters (MIN), and highlight maximum performance thresholds (MAX).
* **Conditional Formatting (Icon Sets):** Applied visual hierarchy triggers to instantly highlight failing parameters, giving HR managers immediate visibility into compliance risks.

---

### 3. Dynamic Automated Corporate Payroll
* **Location:** `Payroll/Payroll_Example.xlsx`
* **Goal:** Process a multi week monthly hourly payroll registry, accounting for variable hourly wages, overtime thresholds, automated overtime bonus distribution and automated weekly totals.

#### ⭐ Actions & Functions Used:
* **Conditional Overtime Layering:** Monitored fluctuating weekly standard hours. If hours exceeded standard capacity (40 hours), the sheet isolated the remainder and mapped it directly into an `Overtime Hours` tier.
* **Financial Calculations:** Calculated standard base wages and applied a 1.5x multiplier calculation pattern for the `Overtime Bonus` arrays.
* **Array Based Totaling (`SUM` / Relative References):** Automated dynamic horizontal row calculations across the spreadsheet to marry base pay and overtime bonuses cleanly into a 5 week `Total` payout matrix.
* **Summary Analytics (`SUM`, `AVERAGE`, `MIN`, `MAX`):** Built a multi layered executive baseline at the base of the sheet to track organizational performance parameters instantly:
  * **`SUM`:** Aggregated massive vertical monthly payout columns into a consolidated financial total for effortless accounting export.
  * **`AVERAGE` / `MAX` / `MIN`:** Monitored floor level workforce data, instantly isolating core metrics such as peak individual earnings (`MAX`), baseline payroll floors (`MIN`), and mean hour trends (`AVERAGE`).
---

## Why These Implementations Matter

1. **Data Integrity:** By utilizing locked down logical statements (`IF`, `AND`, `OR`), I eliminated manual input errors, ensuring that calculations like payroll bonuses or warranty statuses remain 100% accurate.
2. **Scalability:** The formulas are written using relative and absolute cell references (`$`), meaning hundreds of new rows of cars or employees can be added seamlessly without breaking the sheets.
3. **Executive Visibility:** Through the use of Pivot tables and highlighted formatting, complex table data is converted into decision ready business intelligence.
