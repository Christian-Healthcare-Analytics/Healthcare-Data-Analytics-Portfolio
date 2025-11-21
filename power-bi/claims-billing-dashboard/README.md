# 💰 Claims & Billing Dashboard (Power BI)
Tracks financial performance across payers, denials, claims aging, billed vs paid, and financial risk indicators.

## Tools
Power BI • DAX • Data Modeling • Healthcare Revenue Cycle Data

## Dataset Files
- claims.csv
- encounters.csv
- payers (auto generated inside claims)

## Metrics
- Total Billed Amount  
- Total Paid Amount  
- Denial Rate (%)  
- Common Denial Reasons  
- Payments by Payer  

## DAX Sample
```DAX
Denial Rate % =
DIVIDE(
    CALCULATE(COUNT(claims[claim_id]), claims[status] = "Denied"),
    COUNT(claims[claim_id])
)

