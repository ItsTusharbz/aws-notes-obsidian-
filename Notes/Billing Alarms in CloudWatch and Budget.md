
- Billing data metric is stored in CLoudWatch us-east-1
- Billing data are for overall worldwide AWS costs
- It's for actual cost, not for project costs

- Intended for simple alarm (not for powerful AWS Budgets)


#### AWS Budget
- Create a budget and send alarm when cost exceeds the budget.
- 4 types of budgets : Usage, cost, Reservation, Saving Plans
- For reserve instance (RI):
  - Track utilisation
  - Support EC2, Elasticache, RDS, Redshift.
- Upto 5 SNS notification per budget
- Can filter by : service, tag, location , AZ , Purchase Options, Instance Type, Region, API operations
- Same options as cost explorer
- 2 budget are free then $0.02/day/budget.
