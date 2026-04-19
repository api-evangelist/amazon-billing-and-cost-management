# Amazon Billing And Cost Management

AWS Billing and Cost Management is a suite of tools and APIs that enables organizations to view, analyze, forecast, budget, and optimize their AWS spending. It includes AWS Cost Explorer for cost analysis and forecasting, AWS Budgets for budget tracking and automated actions, Cost Anomaly Detection for ML-powered anomaly identification, Cost Categories for spend organization, and the AWS Price List API for programmatic pricing queries.

**Human URL:** [https://aws.amazon.com/aws-cost-management/](https://aws.amazon.com/aws-cost-management/)

**Console:** [https://console.aws.amazon.com/cost-management/](https://console.aws.amazon.com/cost-management/)

## APIs

### AWS Cost Explorer API
Programmatic access to query, filter, group, and analyze cost and usage data with forecasting and optimization recommendations.

**Base URL:** `https://ce.us-east-1.amazonaws.com`

### AWS Budgets API
Create and manage cost, usage, and commitment coverage budgets with threshold notifications and automated enforcement actions.

**Base URL:** `https://budgets.amazonaws.com`

### AWS Price List API
Query AWS service pricing in JSON or CSV format programmatically.

**Base URL:** `https://pricing.us-east-1.amazonaws.com`

#### Key Operations

| Operation | Description |
|---|---|
| GetCostAndUsage | Query cost and usage by service, account, tag, region |
| GetCostForecast | Generate cost forecasts based on historical patterns |
| CreateAnomalyMonitor | Set up ML-powered cost anomaly detection |
| GetAnomalies | List detected cost anomalies |
| GetRightsizingRecommendation | Get EC2 rightsizing recommendations |
| GetSavingsPlansPurchaseRecommendation | Get Savings Plans recommendations |
| CreateBudget | Create a cost or usage budget with notifications |
| CreateBudgetAction | Automate responses when budget thresholds are exceeded |
| CreateCostCategoryDefinition | Map costs to organizational categories |

## Features

- **Cost and Usage Analysis** — Query cost data by service, account, tag, region, and other dimensions
- **Cost Forecasting** — ML-based cost and usage forecasts for budget planning
- **Cost Anomaly Detection** — Automated detection of unusual spending with SNS/email alerts
- **Budgets and Actions** — Custom budgets with automated enforcement via IAM, SCP, or SSM
- **Rightsizing Recommendations** — Identify idle and underutilized EC2 instances
- **Savings Plans and RI Recommendations** — Compute commitment purchase recommendations
- **Cost Categories** — Map AWS costs to teams, projects, and environments for chargeback

## Use Cases

- **FinOps Cost Monitoring** — Centralized cost visibility across accounts with anomaly detection
- **Budget Governance** — Automated spending controls with budget actions
- **Chargeback/Showback** — Internal cost allocation by team, project, or environment
- **Cost Optimization** — Rightsizing, Savings Plans, and Reserved Instance recommendations

## Artifacts

| Type | URL |
|---|---|
| OpenAPI (Cost Explorer) | [openapi/aws-cost-explorer-api-openapi.yml](openapi/aws-cost-explorer-api-openapi.yml) |
| OpenAPI (Budgets) | [openapi/aws-budgets-api-openapi.yml](openapi/aws-budgets-api-openapi.yml) |
| JSON Schema (Budget) | [json-schema/cost-budget-schema.json](json-schema/cost-budget-schema.json) |
| JSON Structure | [json-structure/billing-resource-structure.json](json-structure/billing-resource-structure.json) |
| JSON-LD Context | [json-ld/context.jsonld](json-ld/context.jsonld) |
| Spectral Ruleset | [spectral/ruleset.yml](spectral/ruleset.yml) |
| Capabilities | [capabilities/capabilities.yml](capabilities/capabilities.yml) |
| Vocabulary | [vocabulary/vocabulary.yml](vocabulary/vocabulary.yml) |
| Examples | [examples/](examples/) |

## Common Properties

| Type | URL |
|---|---|
| Documentation | [https://docs.aws.amazon.com/cost-management/latest/userguide/](https://docs.aws.amazon.com/cost-management/latest/userguide/) |
| Pricing | [https://aws.amazon.com/aws-cost-management/pricing/](https://aws.amazon.com/aws-cost-management/pricing/) |
| FAQ | [https://aws.amazon.com/aws-cost-management/faqs/](https://aws.amazon.com/aws-cost-management/faqs/) |
| Blog | [https://aws.amazon.com/blogs/aws-cloud-financial-management/](https://aws.amazon.com/blogs/aws-cloud-financial-management/) |

## Maintainers

**Kin Lane** — [kin@apievangelist.com](mailto:kin@apievangelist.com)
