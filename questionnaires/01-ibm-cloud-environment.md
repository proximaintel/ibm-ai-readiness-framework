# IBM Cloud Environment Assessment

## Purpose
Evaluate the current IBM Cloud infrastructure foundation and its readiness to support enterprise AI workloads.

## Questions

### Account & Organization Structure
1. Do you use IBM Cloud with multiple resource groups? (Yes/No)
2. Is IBM Cloud Enterprise configured for multi-account management? (Yes/No)
3. How many IBM Cloud accounts are in your organization? (1-5 / 6-20 / 21+)
4. Are environments segmented (dev/staging/prod)? (1-5 scale)
5. Are IAM access groups and policies enforced? (Yes/No)

### Infrastructure
6. Is VPC infrastructure deployed? (Yes/No)
7. Are workloads running on Red Hat OpenShift (ROKS)? (Yes/No)
8. Is IBM Cloud Satellite configured for hybrid/edge? (Yes/No)
9. Are private endpoints configured for IBM Cloud services? (Yes/No)
10. Is Transit Gateway used for cross-VPC connectivity? (Yes/No)

### Identity & Access
11. Is IBM Cloud IAM integrated with an external IdP (Okta, Entra ID)? (Yes/No)
12. Is MFA enforced for all users? (Yes/No)
13. Are service IDs scoped to specific resources? (1-5 scale)
14. Is Activity Tracker enabled for audit logging? (Yes/No)

### Compute & Automation
15. What compute services are primarily used? (VPC VSIs / ROKS / Code Engine / Satellite / Mixed)
16. Is infrastructure managed as code (Terraform/Schematics)? (1-5 scale)

## Scoring Weight
This section contributes **20%** to the overall AI Readiness Score.
