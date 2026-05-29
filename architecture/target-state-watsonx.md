# Target State: watsonx.ai in Regulated Environments

## Architecture Overview

```
┌─────────────────────────────────────────────────────────────┐
│                IBM Cloud Account (AI Workloads)               │
│                                                             │
│  ┌──────────────┐   ┌──────────────┐   ┌──────────────┐   │
│  │ watsonx.ai   │   │ watsonx.data │   │ watsonx      │   │
│  │ (Foundation  │   │ (Lakehouse)  │   │ .governance  │   │
│  │  Models)     │   │              │   │ (AI Gov)     │   │
│  └──────┬───────┘   └──────┬───────┘   └──────────────┘   │
│         │                  │                                │
│  ┌──────┴──────────────────┴───────┐                       │
│  │      Private Endpoints          │                       │
│  │  (watsonx, COS, Key Protect)   │                       │
│  └──────────────┬──────────────────┘                       │
│                 │                                           │
│  ┌──────────────┴──────────────────┐                       │
│  │        VPC (Private Subnets)    │                       │
│  │   (no internet, TGW attached)   │                       │
│  └─────────────────────────────────┘                       │
│                                                             │
└─────────────────────────────────────────────────────────────┘
         │
         │ Transit Gateway
         ▼
┌─────────────────────┐     ┌─────────────────────┐
│ Data Account        │     │ Security Account    │
│ (Cloud Object       │     │ (Security &         │
│  Storage, Db2,      │     │  Compliance Center, │
│  Event Streams)     │     │  Activity Tracker)  │
└─────────────────────┘     └─────────────────────┘
```

## Key Components

### watsonx.ai
- Foundation models: Granite, Llama, Mixtral
- Prompt Lab for prompt engineering and testing
- Tuning Studio for model fine-tuning with enterprise data
- Deployed via private endpoints — no public internet access

### watsonx.data
- Open lakehouse architecture (Iceberg, Parquet)
- Presto/Spark query engines
- Integration with existing Db2 and data warehouse
- Cost optimization through tiered storage

### watsonx.governance
- AI Factsheets for model documentation
- Drift detection and model monitoring
- Bias detection and fairness metrics
- Regulatory compliance reporting (EU AI Act, OCC AI guidance)

### Security
- Private endpoints for all watsonx services
- Key Protect (or Hyper Protect for FIPS 140-2 Level 4)
- Activity Tracker for all API calls
- Security & Compliance Center with FS Cloud profile

### Compliance Considerations
- IBM Cloud for Financial Services (FS Cloud) validated
- Data never leaves the IBM Cloud region
- Model invocation logs retained per compliance requirements
- AI Factsheets provide audit trail for model lifecycle
