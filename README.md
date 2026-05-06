#  LEGO Sets Business Analysis (Power BI Project)

##  Business Problem

LEGO offers thousands of products across different themes, price ranges, and target age groups. Understanding which products drive revenue and how pricing, pieces, and themes influence performance is essential for improving product strategy and sales planning.

This project analyzes LEGO sets from both a **product perspective (real data)** and a **sales perspective (simulated data)** to generate actionable business insights.

---

##  Dataset Overview

This project uses **two datasets**:

###  Real LEGO Dataset (Product Analysis)

* Contains actual LEGO set information
* Fields: Set ID, Name, Theme, Subtheme, Category, Year, Pieces, Price, Age Range

---

###  Generated Sales Dataset (Business Simulation)

* Created using Python script (`generate_sales_data.py`)
* Fields include:

  * Estimated Units Sold
  * Region (USA, Europe, Asia-Pacific)
  * Sales Channel (Online, Retail)
  * Discount %

>  Note: Sales dataset is simulated for analytical and learning purposes.

---

##  Data Cleaning & Preparation

* Removed records with missing or inconsistent values to ensure data reliability
* Filtered dataset to include complete and usable records for dashboard consistency
* Standardized data types (Year → Numeric, IDs → Text)
* Handled missing values appropriately

### Feature Engineering:

* **Revenue = Price × Estimated Units Sold**
* **Revenue After Discount**
* **Discount Impact % = (Revenue - Revenue After Discount) / Revenue**

---

## Python Data Generation

The file `generate_sales_data.ipynb` was used to simulate realistic sales data based on product attributes.

### Key Logic:

* Units sold estimated based on price and product complexity
* Regions assigned (USA, Europe, Asia-Pacific)
* Sales channels distributed (Online, Retail)
* Discount percentages applied (0–20%)

This approach allows simulation of real-world business scenarios for analysis.

---

##  Dashboard Structure

###  Product Exploration Dashboard (Real Data)

* Total Sets, Avg Price, Avg Pieces, Avg Age
* Product-level exploration with filters and images

---

###  Revenue Insights Dashboard (Simulated Data)

* Total Revenue: $11.73Bn
* Total Units Sold: 485M
* Discount Impact: 10.58%
* Top Region: Asia-Pacific

---

##  Key Insights

* Licensed themes generate the highest revenue → Expand product lines
* High-piece sets drive more revenue → Focus on premium sets
* Asia-Pacific is top-performing region → Strengthen regional strategy
* Discounts reduce revenue → Use targeted discounting
* Online & Retail channels balanced → Maintain omnichannel approach
* Age group 5–8 is core segment → Expand offerings
* Revenue shows declining trend → Introduce innovation

---

## Dashboard Features

* Interactive filters (Theme, Age, Price)
* Drill-down hierarchy
* Page navigation
* Visual storytelling

---

##  Tools Used

* Power BI
* Python
* DAX
* Data Modeling

---

##  Conclusion

This project combines real product data with simulated sales data to analyze LEGO business performance. Key drivers include licensed themes, product complexity, and regional demand, while discount strategies and trends highlight optimization opportunities.

---

## 📸 Dashboard Preview

### Overview

![Overview](screenshots/overview.png)

### Explore

![Explore](screenshots/explore.png)

### Insights

![Insights](screenshots/insights.png)

---

##  Repository Structure


LEGO-PowerBI-Analysis/
│── lego.pbix
│── lego_dataset.csv
│── sales_dataset_generated.csv
│── generate_sales_data.py
│── README.md
│── screenshots/
│     ├── overview.png
│     ├── explore.png
│     ├── insights.png
```

---

##  How to Use

1. Download the `.pbix` file
2. Open in Power BI Desktop
3. Explore dashboards using filters and navigation

---
