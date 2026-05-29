# Security & Compliance Assessment

## Purpose
Evaluate the security posture and compliance readiness for AI workloads on IBM Cloud.

## Questions

### Security Services
1. Is IBM Cloud Security & Compliance Center enabled? (Yes/No)
2. Are compliance profiles configured (FS Cloud, HIPAA, SOC 2)? (Yes/No)
3. Is IBM Cloud Activity Tracker enabled for all accounts? (Yes/No)
4. Is Flow Logs enabled for VPC traffic monitoring? (Yes/No)
5. Is IBM Cloud Monitoring (Sysdig) deployed? (Yes/No)

### Encryption & Data Protection
6. Is Key Protect used for encryption key management? (Yes/No)
7. Is Hyper Protect Crypto Services used for FIPS 140-2 Level 4? (Yes/No)
8. Is encryption at rest enforced for all data stores? (Yes/No)
9. Is encryption in transit enforced (TLS 1.2+)? (Yes/No)
10. Are private endpoints used for all IBM Cloud services? (Yes/No)

### Compliance
11. Which compliance frameworks apply? (HIPAA / SOC 2 / PCI-DSS / FedRAMP / FS Cloud / NIST / Other)
12. Are compliance controls automated via Security & Compliance Center? (1-5 scale)
13. Is IBM Cloud for Financial Services (FS Cloud) validated? (Yes/No/In Progress)

### AI-Specific Security
14. Is watsonx.governance configured for model monitoring? (Yes/No/N/A)
15. Are AI model access logs captured and monitored? (Yes/No)

## Scoring Weight
This section contributes **20%** to the overall AI Readiness Score.
