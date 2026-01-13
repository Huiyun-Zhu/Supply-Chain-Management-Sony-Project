Supply Chain Management Project — Sony WH-1000XM5
This repository contains a supply chain management project that analyzes Sony’s competitive positioning and applies end-to-end production and inventory planning methods to a selected product: Sony WH-1000XM5 headphones.
Sony’s success in consumer electronics is closely tied to innovation, user-centered design, and a strong (often vertically integrated) supply chain. By tightly aligning product design, engineering, and operations, Sony is able to deliver a consistent user experience while responding to evolving consumer expectations. This project evaluates how production, demand, and inventory decisions can be structured to support that strategy.
Focus Product
• Product: Sony WH-1000XM5
• Scope: Demand forecasting → aggregate planning → master production schedule (MPS) → material requirements planning (MRP) → inventory policy design
⸻
What’s Included
• PPT: Project presentation (key insights and decisions)
• Excel: Forecasting + planning models (calculations and scenarios)
• Report: Written analysis and methodology
⸻
Key Analyses & Methods
1) Demand Planning (Forecasting)
Demand is forecasted using the Holt–Winters model to capture seasonality and peaks (notably Christmas / New Year).
• Validation performance: MAPE = 3.98%
• Purpose: Translate forecasted demand into production, supply, and inventory decisions.
2) Aggregate Production Planning
Several aggregate plans are compared. The hybrid plan is selected as the best overall trade-off:
• Total cost: $28.474M
• Only ~15% more expensive than the cheapest option (level plan),
while avoiding major drawbacks such as:
• limited ability to handle additional orders (risk of missed sales),
• relatively high outsourcing costs,
• less favorable ethical implications compared to a pure chase approach.
3) Detailed Planning: MPS & MRP
After the aggregate plan, a detailed Master Production Schedule (MPS) is derived.
Then, Material Requirements Planning (MRP) is used to compute dependent demand for subcomponents based on the BOM, including backward planning for child components.
4) Inventory Planning Models
Multiple inventory approaches are evaluated, including:
• EOQ / EPQ
• Quantity discount model
• Safety stock
• Periodic review model
• Single-period inventory model
Considering discounts on a key component (charging circuitry), the MRP policy can be adapted to order 300,000 units every two weeks, achieving an estimated 10% unit cost reduction, which outweighs the additional holding costs.
Final recommendation: The periodic review model is selected as the best fit for WH-1000XM5, with a review cadence aligned to a ~9-day review period (weekly planning rhythm).
⸻
How to Use This Repo
1. Start with the PPT for the narrative and decisions.
2. Open the Excel models to explore:
• forecasting setup and validation,
• scenario comparisons for aggregate planning,
• MPS/MRP logic and outputs,
• inventory policy parameters and sensitivity.
3. Read the report for full explanations, assumptions, and conclusions.
⸻
Notes
This project is for academic/learning purposes. Cost figures and policies are based on the assumptions and dataset used in the models included in this repository.
⸻
