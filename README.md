# SQL Code outlining how analysis was carried out to identify the top 5 Projects exceeding their budget 

Columns:
project_id: Unique identifier for each project.
project_name: Descriptive name of the project.
planned_cost: The estimated cost allocated for the project during planning.
budget: The financial threshold or limit set for the project.
actual_cost: The real expense incurred for the project, sourced from the Costs table.
percent_over_budget: A calculated metric showing how much the project overspent as a percentage of its budget.
total_exceeding_budget: The absolute amount by which the project exceeded its budget, calculated as actual_cost - budget when over-budget.
rank: The ranking of projects based on total_exceeding_budget in descending order.

Tables Used:
Projects: Provides the primary project details (project_id and project_name).
Costs: Supplies the actual cost (actual_cost) associated with each project.
Budgets: Includes financial details like planned_cost and budget.
