
# Global Bike Sales & Profitability Analysis

## Objective
The objective of this project was to analyze transactional retail data for a global bicycle distributor to evaluate sales performance, regional demand, and product profitability. By leveraging key financial columns (Unit Cost, Unit Price, Profit) alongside demographic and geographic data, this analysis provides actionable business insights to optimize inventory management, refine pricing strategies, and target high-value customer segments.

## Data Source & Structure
 Dataset: Global Bike Sales Dataset (Kaggle)
 Granularity: 1,000+ individual sales transactions
 Core Attributes Analyzed:
 Temporal: Date, Month, Year
 Demographic: Gender, Age Group
 Geographic: Country, State
Product Hierarchy: Product Category, Sub Category, Product
 Financial Metrics: Order Quantity, Unit Cost, Unit Price, Profit

## Data Cleaning & Preparation
Before analyzing the data, the following data cleaning steps were performed using Excel / Power Query:
 Removed Duplicates: Identified and removed duplicate rows to ensure data integrity.
 Calculated Columns:
 Total Revenue: Created a calculated measure using Order Quantity * Unit Price.
Total Cost: Created a calculated measure using Order Quantity * Unit Cost.
Profit Margin (%): Established a formula to calculate relative profitability: $\text{Profit Margin} = \frac{\text{Profit}}{\text{Total Revenue}} \times 100$.
 Data Integrity Checks: Verified that the pre-calculated Profit column perfectly matched the calculated values ($\text{Revenue} - \text{Cost}$) across all rows.
 Data Formatting: Standardized financial metrics into local currencies and formatted temporal fields for smooth time-series sorting.
 Created Age Brackets: Used a nested IF formula to group customers into distinct life stages for better demographic targeting:
 Youth: Under 25
 Young Adut: 25 to 34
 Adult: 35 to 64
 Senior: 65 and above

# Key Features & Tools Used
 Data Transformation: Conditional formatting, nested logic formulas (IF), and text cleaning functions.

 Pivot Tables: Built to aggregate financial and demographic metrics dynamically across multiple dimensions (e.g., tracking total profit by state and year).

 Interactive Dashboard: Combined dynamic charts with interactive Slicers for Region, Education, and Marital Status, allowing stakeholders to filter data on the fly.

## Key Insights 
Based on exploratory analysis of this sales data, several critical trends emerge:

* **High Volume vs. High Value:** `Accessories` (like helmets and tires) and `Clothing` make up the vast majority of the **Order Quantity**, but `Bikes` generate over 70% of the total **Revenue**.
* **Demographic Hotspots:** The core customer demographic is concentrated in the **Young Adult (25-34)** and **Adult (35-64)** segments. Gender distribution remains relatively balanced across most categories, though men slightly edge out women in high-end mountain bike purchases.
* **Geographic Drivers:** High-income states (e.g., California in the US, New South Wales in Australia) act as primary revenue engines, especially for premium bike models.
* **Seasonality:** Sales experience noticeable spikes during Q2 (Spring/Summer ramp-up) and Q4 (Holiday gifting season).


##  Recommendations

### 1. Optimize Pricing and Bundling
* **The Strategy:** Since `Accessories` have a low unit cost but high order volume, use them as low-cost incentives. 
* **Action:** Implement "Complete the Ride" product bundles at checkout. For example, offer a 10% discount on a helmet and water bottle cage when a customer purchases a high-value `Bike`.

### 2. Targeted Demographic Marketing
* **The Strategy:** Capitalize on the purchasing power of the 25–64 age demographic.
* **Action:** Direct digital ad spend toward this segment highlighting premium comfort and performance lines. Concurrently, introduce entry-level, budget-friendly commuter options targeted at the under-25 (`Youth`) segment to cultivate early brand loyalty.

### 3. Inventory and Supply Chain Forecasting
* **The Strategy:** Minimize stockouts of high-demand items during peak seasons.
* **Action:** Align inventory procurement cycles with the Q2 and Q4 seasonal surges. Ensure safety stock for top-selling sub-categories (like tires and tubes) is replenished at least 30 days prior to these peak windows.

### 4. Regional Product Allocation
* **The Strategy:** Tailor product availability to regional demand profiles.
* **Action:** Allocate high-margin, specialized inventory (e.g., expensive carbon-frame road or mountain bikes) heavily to top-performing states like California, while focusing on essential commuter gear in dense urban regions.

## Interactive Dashboard 


This is my first project using Excel for data analysis to analyze a bike sales dataset
