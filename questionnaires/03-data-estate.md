# Data Estate Assessment

## Purpose
Evaluate the data platform maturity and readiness to support AI workloads on IBM Cloud.

## Questions

### Data Storage & Architecture
1. Is watsonx.data deployed as the lakehouse platform? (Yes/No/Evaluating)
2. Is Cloud Pak for Data used for data management? (Yes/No)
3. What databases are in use? (Db2 / PostgreSQL / MongoDB / Netezza / Other)
4. Is a medallion or layered architecture implemented? (Yes/No)
5. Is data stored in IBM Cloud Object Storage? (Yes/No)

### Data Governance
6. Is Watson Knowledge Catalog deployed? (Yes/No)
7. Is data lineage tracked? (Yes/No/Partial)
8. Is data classified by sensitivity level? (Yes/No)
9. Are data access policies enforced centrally? (1-5 scale)
10. Are data retention policies defined and enforced? (Yes/No)

### Data Quality
11. Are data quality checks automated in pipelines? (Yes/No)
12. What is the estimated data quality score? (1-5 scale)
13. Are data freshness SLAs defined? (Yes/No)

### Integration
14. How many source systems feed the data platform? (1-5 / 6-20 / 20+)
15. Are real-time/streaming pipelines in use (Event Streams/Kafka)? (Yes/No)

## Scoring Weight
This section contributes **20%** to the overall AI Readiness Score.
