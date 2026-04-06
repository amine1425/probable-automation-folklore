# Reporting Challenges for Nasamotor — Comparative Study

## Context

Business users at Nasamotor are independently building Power BI reports using manual extracts from the core system (Autoline DMS and others).

**Consequences:**
- Report inconsistency
- Limited governance
- Lack of unified metrics/KPIs
- Redundancy
- Increased risk of error or non-compliance

## Target

Develop a centralized, scalable, and controlled approach to data and reporting for analytics, decision-making, and compliance.

---

## Scenario 1: Standard Data & BI Approach ("Modern BI Stack")

### Steps

1. Build an enterprise-grade data lake (Azure Data Lake) that connects all data sources (Autoline, HR SQL export, SharePoint, Power Apps, manual sources).
2. Set up data governance rules, data catalog (data dictionary), lineage, and access controls (e.g., Azure Purview).
3. Implement a standardized, centralized Power BI reporting framework — shared datasets, certified dashboards, and referential data models.
4. Define granular access rights by role/group to ensure data security, GDPR compliance, and business separation.

### Tree Map (Capacities)

- **Data Lake** (raw, curated layers)
  - Core systems (Autoline, HR, finance)
  - External/Manual (Excel, SharePoint)
- **Data Governance**
  - Metadata management
  - Access control
  - Data quality
- **Power BI Layer**
  - Certified Datasets
  - Standard dashboards
  - Workspace management
- **User Management**
  - Audit, RBAC

### Values

- **TRUST** in numbers — one source of truth
- **AUDITABILITY** for regulatory/AML compliance
- Control over **GDPR** and sensitive views
- **Efficiency** — less rework, fewer errors
- **Scalability** — easy to expand for new sources or metrics

### Impacts / KPIs

| KPI | Description |
|-----|-------------|
| % reduction in report errors | Measures data quality improvement post-implementation |
| % Power BI usage on certified datasets | Tracks adoption of the governed reporting layer |
| Time to deploy a new KPI/metric | Measures agility of the BI team |
| # of unique dashboards maintained | Tracks consolidation and rationalization |
| Data SLA compliance | Measures reliability and freshness of data pipelines |

---

## Scenario 2: AI-Driven Reporting & Analytics Approach

### Steps

1. Build the same data lake & governance foundation as Scenario 1.
2. Add AI/ML layer: Natural Language Query tools (e.g., Power BI Copilot, Azure OpenAI), smart anomaly detection, predictive analytics, automatic report generation.
3. User experience focused on conversational and self-service analytics — business users ask questions and get dynamic, story-based answers.
4. ML-driven custom alerts, root cause analysis, voice/WhatsApp data query integration.

### Tree Map (Capacities)

- **Data Lake**
- **Data Governance** (as above)
- **AI/ML Layer**
  - Auto-insights (trends, anomalies)
  - Natural Language Query (NLQ/Chat)
  - Predictive models (sales, inventory, risk)
  - Automated narrative reports
- **Advanced User Experience**
  - Dynamic dashboard customization
  - Conversational UI, not just static filters
  - Multilingual/voice/WhatsApp access

### Values

- Higher **BUSINESS AGILITY** — all users can answer new questions instantly
- Lower IT overhead — central team builds foundations, business users are self-serve
- More proactive insight discovery (AI escalates what humans might miss)
- Accelerated adoption of ML/advanced analytics without hiring large data teams

---

## Scenario Comparison

| Aspect | Standard BI | AI-Driven BI |
|--------|-------------|--------------|
| Data Foundation | Data lake, governance | Same |
| User Interaction | Build reports, click filters | Ask, converse, auto-generate |
| Insights | Static dashboards | Dynamic, stories, predictive |
| ML/AI | Manual analytics | Anomalies + predictions |
| Error Rates | Lower after setup | Even lower (proactive) |
| IT/Developer Workload | Ongoing support | Reduced (self-serve) |
| Cost (TCO) | Initial + ongoing maintenance | More initial AI investment, less later |
| KPIs Managed | Centralized set | Expanded, ad-hoc, evolving |
| Governance/Compliance | Strong | Strong (with monitoring) |

### AI/ML Impact (Scenario 2)

- More frequent, actionable alerts (sales drops, fraud patterns, AML triggers)
- Natural language summaries for board reporting & compliance
- Predict sales trends, optimize inventory, catch anomalies in payment/fraud

### KPI / Cost / Value Impact (Scenario 2)

| KPI | Description |
|-----|-------------|
| % of insights delivered without IT/dev intervention | Measures self-service effectiveness |
| Rate of business decision cycle times (faster) | Measures speed of insight-to-action |
| # of user-initiated KPI definitions per quarter | Tracks business empowerment |
| Lower dashboard maintenance hours | Measures IT overhead reduction |
| Direct cost: AI service fees vs traditional IT | Tracks TCO evolution |

---

## Recommendation

**Start with Scenario 1** for rapid trust + compliance, then **layer in Scenario 2** for a step-change in user empowerment and actionable, ML-driven insights.

This phased approach allows Nasamotor to:
1. Build the governance and data foundation first — ensuring data quality, GDPR compliance, and auditability.
2. Progressively introduce AI/ML capabilities as the organization's data maturity and user readiness grow.
3. Realize quick wins from centralized reporting while building toward advanced analytics.

---

## Appendix

### A. Sample Capacity Trees

**Scenario 1 — Modern BI Stack**

```
Azure Data Lake
├── Raw Layer
│   ├── Autoline DMS (core transactions)
│   ├── HR SQL Export
│   ├── Finance system
│   └── Manual sources (Excel, SharePoint)
├── Curated Layer
│   ├── Cleaned & validated datasets
│   └── Business-ready data models
└── Serving Layer
    └── Power BI Certified Datasets

Azure Purview (Governance)
├── Data Catalog / Dictionary
├── Lineage Tracking
└── Access Control Policies

Power BI Premium
├── Certified Dashboards
│   ├── Sales & Revenue
│   ├── Aftersales & Workshop
│   ├── HR & Headcount
│   └── Finance & Compliance
├── Shared Semantic Models
└── Workspace RBAC
```

**Scenario 2 — AI-Driven BI**

```
(All of Scenario 1, plus:)

AI/ML Layer (Azure OpenAI / Fabric)
├── Natural Language Query (Power BI Copilot)
├── Anomaly Detection (sales drops, fraud signals)
├── Predictive Models
│   ├── Sales forecasting
│   ├── Inventory optimization
│   └── AML risk scoring
└── Automated Narrative Reports

Advanced UX
├── Conversational Analytics (chat, voice)
├── WhatsApp / Teams integration
└── Multilingual interface
```

### B. Stakeholder Value Impacts

| Stakeholder | Scenario 1 Value | Scenario 2 Value |
|-------------|-----------------|-----------------|
| C-Suite / Board | Trusted, auditable numbers for decisions | Proactive alerts + predictive board reports |
| Finance | GDPR-compliant, reconcilable reports | AI-driven anomaly detection in transactions |
| Sales Management | Single source of truth for pipeline & revenue | Predictive sales alerts & opportunity scoring |
| Workshop / Aftersales | Standardized KPIs | Predictive maintenance scheduling insights |
| HR | Consolidated workforce analytics | Turnover prediction models |
| Compliance / AML | Auditable, lineage-tracked reports | AI-triggered AML alerts (Law 83/2017) |
| IT Team | Governed, centralized infrastructure | Reduced maintenance, self-serve empowerment |
| Business Users | Reliable certified dashboards | Self-service NLQ — ask any question instantly |

### C. Phased Transition Roadmap

```
Phase 1 (0–6 months): Foundation & Governance
├── Deploy Azure Data Lake (raw + curated layers)
├── Connect Autoline DMS, HR SQL, Finance
├── Set up Azure Purview (catalog, lineage, access)
├── Migrate priority reports to certified Power BI datasets
└── Define RBAC model and workspace governance

Phase 2 (6–12 months): Standardization & Adoption
├── Decommission redundant manual reports
├── Train business users on certified dashboards
├── Expand data sources (SharePoint, Power Apps, Excel)
├── Publish data dictionary and data quality SLAs
└── Establish BI Center of Excellence (CoE)

Phase 3 (12–24 months): AI-Driven Layer
├── Enable Power BI Copilot / Azure OpenAI integration
├── Deploy anomaly detection models (sales, payments, AML)
├── Launch NLQ / conversational analytics for business users
├── Build predictive models (sales forecast, inventory, risk)
└── Automate executive narrative reports and board packs
```

---

*Document prepared as part of the Nasamotor Digital & Analytics Transformation Program.*
*Last updated: April 2026*
