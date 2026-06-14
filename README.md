# Data Analytics & Operations: Excel Portfolio

Welcome to my Excel Portfolio repository. This repository features three distinct business and operational projects designed to solve real-world tracking, management, and financial reporting challenges. 

Each project showcases my proficiency in data modeling, logical and financial formulas, conditional formatting, and building robust, automated worksheets.

---

## 🚀 Projects Overview

### 1. Car Inventory & Fleet Management
* **File Location:** `Car_Inventory/Car_Inventory_Example.xlsx`
* **Objective:** Manage a company vehicle fleet, track mileage usage per driver, assess asset age, and automate warranty coverage tracking.

#### 🔧 Key Actions & Functions Used:
* **`DATEDIF` / Date Arithmetic:** Calculated vehicle age dynamically based on the manufacturing year to determine asset depreciation cycles.
* **`IF` & `AND` / Logical Formulas:** Automated the `Covered?` column to evaluate if a vehicle's current mileage falls under its specific `Warranty Miles` threshold, returning an instant status ("Yes" vs "Not Covered").
* **String Concatenation (`&` or `CONCAT`):** Developed a standardized `New Car ID` indexing system by combining Make, Model, Color, and unique numeric sequences into a single primary key string.
* **Pivot Tables & Data Summarization:** Constructed a driver mileage breakdown dashboard to track which drivers accumulate the most miles, enabling fleet maintenance forecasting.

---

### 2. Employee Performance & HR Gradebook
* **File Location:** `Gradebook/Gradebook_Example.xlsx`
* **Objective:** Track candidate compliance and training metrics across critical testing criteria (Safety, Philosophy, Financial Skills, and Drug Screenings) to automate operational HR decisions.

#### 🔧 Key Actions & Functions Used:
* **Percentage Scaling & Normalization:** Converted raw point results into clean decimal percentages based on dynamically referenced "Points Possible" headers.
* **Multi-Criteria Evaluation (`IF`, `OR`):** Built the `Fire Employee? True / False` logic gate. The formula flags `True` if an employee fails a zero-tolerance compliance test (like the Drug Test) or if their core performance drops below the minimum acceptable business standard.
* **Conditional Formatting:** Applied visual hierarchy triggers to instantly highlight failing parameters, giving HR managers immediate visibility into compliance risks.

---

### 3. Dynamic Automated Corporate Payroll
* **File Location:** `Payroll/Payroll_Example.xlsx`
* **Objective:** Process a multi-week monthly hourly payroll registry, accounting for variable hourly wages, overtime thresholds, and automated overtime bonus distribution.

#### 🔧 Key Actions & Functions Used:
* **Conditional Overtime Logic:** Used relational formulas to look at weekly hours worked. If hours exceeded standard capacity (40 hours), the sheet isolated the remainder and mapped it directly into an `Overtime Hours` tier.
* **Financial Calculations:** Calculated standard base wages and applied a 1.5x multiplier calculation pattern for the `Overtime Bonus` arrays.
* **Matrix Rollups (`SUM`):** Combined individual weekly pay payouts and overtime adjustments into a consolidated `January Pay` column for clean accounting export.

---

## 💡 Why These Implementations Matter (Business Value)

1. **Data Integrity:** By utilizing locked-down logical statements (`IF`, `AND`, `OR`), I eliminated manual input errors, ensuring that calculations like payroll bonuses or warranty statuses remain 100% accurate.
2. **Scalability:** The formulas are written using relative and absolute cell references (`$`), meaning hundreds of new rows of cars or employees can be added seamlessly without breaking the sheets.
3. **Executive Visibility:** Through the use of Pivot tables and highlighted formatting, complex tabular data is converted into decision-ready business intelligence.

---

## 🛠️ How to Review My Work
* **To interact with formulas:** Download the raw `.xlsx` files from their respective folders and open them in Microsoft Excel.
* **To see quick visuals:** Open the provided `.pdf` files within each folder to instantly view the formatting and sheet layouts directly in your browser.
