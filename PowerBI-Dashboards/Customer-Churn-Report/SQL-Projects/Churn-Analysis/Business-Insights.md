# SQL Churn Analysis – Business Insights

## Key Metrics
- Overall churn rate: 18.5%
- High churn among new customers (<3 months)

## Key SQL Insights:
1. Long-tenure users had lowest churn
2. Customers with family plans showed better retention
3. Users with low usage in first month had 2x churn rate

### Sample SQL Query:
```sql
SELECT tenure, churn, COUNT(*) 
FROM customers 
GROUP BY tenure, churn
ORDER BY tenure;
