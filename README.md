# Amazon Billing And Cost Management

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
