# Supply Chain Management Project — Sony WH-1000XM5
This repository contains a supply chain management project focused on **Sony WH-1000XM5 headphones**, covering demand forecasting, production planning, MPS/MRP, and inventory policy design. Deliverables include a **report**, **Excel models**, and a **presentation deck**.
---
## Project Summary
Sony’s success in consumer electronics is strongly linked to **innovation, user-centered design, and supply chain excellence**. By integrating hardware and software to deliver a consistent user experience, Sony is positioned to address rising consumer expectations and industry challenges while staying aligned with its mission of delivering exceptional value.
This project applies key operations and planning methods to support production management of the **WH-1000XM5**, which requires advanced **demand, supply, and inventory planning**.
---
## Key Results
### 1) Demand Forecasting (Holt–Winters)
- Model: **Holt–Winters**
- Captures seasonal peaks such as **Christmas / New Year**
- Validation performance: **MAPE = 3.98%**
- Purpose: align production, supply, and inventory decisions with forecasted demand
### 2) Aggregate Production Planning
Multiple aggregate plans were evaluated. The **hybrid plan** was selected as the best trade-off:
- Total cost: **$28.474M**
- ~**15%** more expensive than the cheapest option (level plan), but:
 - better handles additional orders (lower risk of missed sales)
 - avoids high outsourcing dependence
 - more ethically acceptable than a pure chase plan
### 3) Detailed Planning (MPS & MRP)
- Built a **Master Production Schedule (MPS)**
- Computed dependent demand via **Material Requirements Planning (MRP)**
- Used the **BOM** and backward planning to derive children component requirements
### 4) Inventory Policy Design
Models evaluated:
- EOQ / EPQ
- Quantity discount model
- Safety stock
- Periodic review model
- Single-period inventory model
Discount insight:
- By leveraging discounts on charging circuitry, MRP can be adapted to order
 **300,000 units every 2 weeks**, yielding ~**10%** unit cost savings, which outweighs
 the additional holding costs.
Final recommendation:
- **Periodic review model** as the best fit for WH-1000XM5
- Review cadence: **~9-day review period** (weekly planning rhythm)
---
## Repository Contents
- `ppt/` — presentation deck  
- `excel/` — forecasting + planning models (calculations and scenarios)  
- `report/` — written report (methods, assumptions, discussion)
> If your folders use different names, rename this section to match your repo structure.
---
## How to Use
1. Open the **PPT** for the overall narrative and decisions.
2. Use the **Excel** files to inspect:
  - forecast setup and validation
  - aggregate planning comparison
  - MPS/MRP outputs
  - inventory parameters and scenario impacts
3. Read the **report** for detailed methodology and assumptions.
---
## Notes
This work is for academic/learning purposes. Results depend on the dataset and assumptions embedded in the Excel models.
---
