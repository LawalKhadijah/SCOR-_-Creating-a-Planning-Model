14-Day Raw Meat Planning & Procurement Optimization Tool

![Project Status](https://img.shields.io/badge/Status-Planning-blue) ![Methodology](https://img.shields.io/badge/Methodology-Agile-orange) ![Framework](https://img.shields.io/badge/Framework-SCOR-green) ![Platform](https://img.shields.io/badge/Platform-Microsoft%20Excel-brightgreen)

1. Project Overview

The 14-Day Raw Meat Planning & Procurement Optimization Tool is an Agile-driven, SCOR-aligned supply chain planning solution designed to improve raw material availability, optimize purchasing decisions, reduce inventory costs, and increase planning efficiency.

The tool integrates demand forecasts, work-in-progress (WIP) requirements, raw material inventory, confirmed purchase orders, and supplier information to generate a forward-looking 14-day supply plan.

It will also incorporate a lowest-cost procurement optimization engine to recommend purchasing quantities, suppliers, and delivery schedules while respecting operational constraints.

The ultimate objective is to transition from manual, fragmented planning activities to a standardized, integrated, and data-driven procurement decision-making process.

2. Business Problem

Current raw meat planning and purchasing activities can involve manually consolidating information from multiple sources, including:

Integrated Business Planning (IBP) forecasts.
Production and WIP plans.
Raw material requirements.
Current inventory levels.
Confirmed purchase orders.
Supplier pricing and lead times.
Minimum order quantities (MOQ).
Existing lowest-cost purchasing calculations.

This creates several potential challenges:

Limited visibility of future raw material shortages.
Time-consuming manual planning and calculations.
Difficulty evaluating alternative purchasing strategies.
Potential excess or insufficient inventory.
Fragmented supplier and procurement information.
Limited visibility of total procurement costs.
Inconsistent planning methodologies.

The proposed solution consolidates these inputs into one planning environment.

3. Project Objectives

The project aims to:

Improve raw material availability for production.
Automate 14-day raw material demand calculations.
Integrate inventory and confirmed purchase orders into daily supply projections.
Identify projected shortages and replenishment requirements.
Incorporate supplier lead times, MOQ, order multiples, and capacity constraints.
Integrate the existing business lowest-cost purchasing methodology.
Optimize total procurement and inventory costs.
Improve supplier performance visibility.
Standardize purchasing recommendations.
Establish measurable supply chain performance indicators using SCOR.
4. Project Architecture

The solution is structured around four interconnected pillars.

4.1 Agile Project Management

Agile provides the development methodology.

The tool will be developed incrementally through short development sprints, allowing users to test functionality, provide feedback, and prioritize improvements.

Key practices:

Product backlog management.
Sprint planning.
Incremental development.
User acceptance testing.
Sprint reviews.
Continuous improvement.
4.2 SCOR Framework

The Supply Chain Operations Reference (SCOR) framework provides the supply chain performance and process measurement structure.

The project will focus on five performance attributes:

Performance Attribute	Application
Reliability	Ensure raw materials are available when production requires them.
Responsiveness	Reduce the time required to update demand and purchasing plans.
Agility	Respond effectively to demand changes and supply disruptions.
Cost	Optimize procurement and inventory-related costs.
Asset Management Efficiency	Improve inventory utilization and reduce excess stock.
4.3 14-Day Planning Engine

The planning engine connects demand, WIP, raw material requirements, inventory, and incoming supply.

Its calculation sequence is:

text
IBP Forecast
     |
     v
WIP / Production Plan
     |
     v
Raw SKU Requirements
     |
     v
Current Inventory + Confirmed POs
     |
     v
14-Day Inventory Projection
     |
     v
Shortage and Replenishment Analysis

4.4 Procurement Optimization Engine

The procurement engine evaluates purchasing alternatives to identify the lowest-cost feasible ordering strategy.

The objective is to minimize:

text
Total Cost =
    Material Purchase Cost
  + Freight Cost
  + Additional Procurement Costs
  + Inventory Holding Cost
  + Applicable Shortage Costs


Subject to operational constraints:

Production requirements must be satisfied.
Inventory must respect defined safety stock requirements.
Supplier MOQ must be respected.
Order multiples must be respected.
Supplier capacity must not be exceeded.
Supplier lead times must be considered.
Approved suppliers and material specifications must be maintained.
Required delivery dates must be achieved.

The optimization engine will build on the inventory projection rather than independently calculating demand.

5. Technical Workflow

The model consists of three main calculation stages.

Stage 1: Raw Material Demand Calculation

Convert finished product and WIP requirements into individual raw material SKU requirements.

Example:

Finished/WIP Item	Raw SKU	Requirement
Wiener A	Pork Trim 80/20	12,000 kg
Wiener A	Beef 90/10	6,000 kg
Wiener B	Pork Trim 80/20	8,000 kg
Bologna A	Beef 90/10	5,000 kg

Aggregate requirements by raw SKU and day across the 14-day planning horizon.

Stage 2: Inventory Projection

For each raw SKU, calculate:

text
Projected Ending Inventory =
    Beginning Inventory
  + Confirmed Purchase Orders
  + Recommended Receipts
  - Daily Raw Material Requirements


The calculation identifies:

Projected inventory by day.
Future inventory shortages.
Replenishment dates.
Required purchasing quantities.
Inventory coverage.
Potential production risks.
Stage 3: Lowest-Cost Procurement Optimization

Evaluate supplier combinations and order quantities based on:

Input	Description
Supplier	Approved supplier
Raw SKU	Material being purchased
Price/kg	Supplier purchase price
MOQ	Minimum order quantity
Order Multiple	Required ordering increment
Freight	Transportation cost
Lead Time	Supplier delivery lead time
Capacity	Available supplier capacity
OTIF	On-time, in-full performance
Quality	Supplier quality performance

The engine will evaluate feasible purchasing alternatives and recommend an appropriate combination based on total cost and operational requirements.

6. Excel Workbook Structure

The proposed workbook will contain the following worksheets:

Tab	Worksheet	Purpose
01	Control Panel	Planning parameters and assumptions
02	IBP Forecast	Demand forecast inputs
03	WIP Plan	Production requirements
04	Raw SKU Mapping	Finished product-to-raw material conversion
05	Inventory	Current inventory balances
06	Open POs	Confirmed purchase orders
07	14-Day Supply Plan	Daily inventory projection
08	Supplier Master	Supplier pricing and constraints
09	Cost Optimizer	Lowest-cost procurement calculations
10	Order Recommendations	Recommended purchasing decisions
11	SCOR Dashboard	Supply chain performance metrics
12	Agile Backlog	Development tasks and sprint tracking
7. Agile Development Roadmap

The project will be delivered through five development sprints.

Sprint	Focus	Deliverables
Sprint 1	Demand and Inventory Visibility	Automated 14-day raw material demand and inventory projection
Sprint 2	Purchasing Requirements	Replenishment quantities, order dates and lead-time calculations
Sprint 3	SCOR Performance	KPI dashboard and supplier performance scorecard
Sprint 4	Procurement Optimization	Lowest-cost supplier and purchasing combinations
Sprint 5	Scenario Planning	What-if analysis, alternative strategies and management dashboard
Sprint Acceptance Criteria

Sprint 1: Identify projected raw material shortages across the 14-day horizon.

Sprint 2: Generate purchasing recommendations using lead times, MOQ, order multiples, and safety stock.

Sprint 3: Measure supply chain performance using defined SCOR-aligned KPIs.

Sprint 4: Recommend the lowest-cost feasible procurement strategy.

Sprint 5: Allow planners to evaluate alternative purchasing and supply scenarios.

8. SCOR Performance Measurement

The project will establish a performance scorecard to measure the effectiveness of the planning and procurement process.

Attribute	KPI	Proposed Target
Reliability	Raw Material Availability	≥99%
Reliability	Production Coverage	≥99%
Reliability	Projected Stockout Rate	Reduce
Responsiveness	Planning Cycle Time	Reduce by 50%
Responsiveness	Order Reaction Time	Reduce
Agility	Scenario Response Time	Under 5 minutes
Agility	Demand Change Absorption	≥95%
Cost	Total Procurement Cost	Reduce
Cost	Optimization Gap	Reduce
Asset Efficiency	Excess Inventory	Reduce
Asset Efficiency	Inventory Days of Supply	Optimize
Asset Efficiency	Expired Meat	Reduce

Note: Targets are initial project proposals and must be validated against actual operational baselines and company requirements.

9. Process Maturity Framework

The project will progressively improve planning process maturity.

Level	Maturity	Characteristics
1	Ad Hoc	Manual planning and individual judgment
2	Repeatable	Standard templates and basic calculations
3	Defined	Integrated and standardized planning process
4	Managed / Optimized	Cost optimization, supplier performance and scenario planning
5	Predictive	Predictive planning and continuous improvement

Initial target: Level 3 — Defined

Long-term target: Level 4 — Managed / Optimized

Level 5 represents a potential future development opportunity.

10. Key Project Success Measures

The project will measure success against three primary outcomes.

Outcome	Success Measure
Service Improvement	Target raw material availability of ≥99%
Planning Efficiency	Reduce planning cycle time by 50–75%
Cost Optimization	Reduce procurement and excess inventory costs without compromising production availability

Additional measures will include:

Reduced manual spreadsheet manipulation.
Improved inventory visibility.
Improved supplier performance measurement.
More consistent purchasing decisions.
Faster scenario evaluation.
Improved planning standardization.
11. Proposed Repository Structure
text
raw-meat-planning-optimization/
│
├── README.md
│
├── docs/
│   ├── project-charter.md
│   ├── business-requirements.md
│   ├── solution-architecture.md
│   ├── scor-framework.md
│   └── process-maturity.md
│
├── excel/
│   ├── templates/
│   ├── formulas/
│   └── sample-data/
│
├── agile/
│   ├── product-backlog.md
│   ├── sprint-plan.md
│   └── acceptance-criteria.md
│
├── optimization/
│   ├── business-rules.md
│   ├── supplier-constraints.md
│   └── cost-model.md
│
├── dashboard/
│   └── kpi-definitions.md
│
└── tests/
    ├── demand-validation.md
    ├── inventory-validation.md
    └── optimization-validation.md

12. Future Enhancements

Potential future capabilities include:

Automated IBP and WIP data integration.
Automated purchase order data extraction.
Advanced mathematical optimization.
Supplier risk scoring.
Demand forecasting accuracy analysis.
Predictive shortage alerts.
Automated inventory parameter recommendations.
Power BI management dashboards.
Integration with ERP and procurement systems.
Actual-versus-planned purchasing analysis.
13. Project Vision

The long-term vision is to develop an integrated raw meat supply chain planning and procurement decision-support solution.

The tool will connect demand planning, production requirements, inventory management, supplier sourcing, procurement optimization, and SCOR performance measurement within one standardized planning environment.

The guiding principles are:

Agile — Develop incrementally and continuously improve.
SCOR — Measure and improve supply chain performance.
Planning — Maintain visibility of raw material requirements over a 14-day horizon.
Optimization — Identify the lowest-cost feasible purchasing strategy.
Continuous Improvement — Use actual performance to improve future planning decisions.
14. North Star
Develop an Agile, SCOR-aligned 14-day raw meat planning and procurement optimization tool that improves raw material availability and planning responsiveness while optimizing inventory and total procurement costs.

The ultimate goal: Right raw material. Right quantity. Right supplier. Right time. Lowest practical total cost.
