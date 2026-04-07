# Reporting Challenges — Presentation Deck
## Client: Nasamotor | Topic 1 | 20 Slides

---

## Slide 1 — Title Slide

### Nasamotor Reporting Transformation
**Centralizing Business Intelligence & Analytics**

*Prepared for: Nasamotor Leadership Team*  
*Topic 1: Reporting Challenges — Options, Analysis & Recommendation*  
*Date: April 2026*

---

**What to say:**  
"Good morning / afternoon everyone. Thank you for taking the time to join us today. This presentation covers our findings and recommendations for Topic 1 — Reporting Challenges — as outlined in Riadh's brief following our workshop with the Nasamotor team. We'll walk through the current situation, the two options we've analyzed in depth, and close with a phased recommendation tailored to Nasamotor's context and growth objectives."

---

## Slide 2 — Agenda

**Today's Agenda:**
1. The Current Situation
2. The Target Vision
3. Option 1: Standard BI & Data Approach
4. Option 2: AI-Driven Reporting Approach
5. Financial & Maintenance Analysis
6. Scalability Comparison
7. Recommendation & Roadmap
8. Next Steps

---

**What to say:**  
"We've structured this session to take you from problem to solution. We'll start by aligning on the current pain points, then define what 'good' looks like for Nasamotor, before diving into the two options in detail. We'll compare them across cost, maintenance and scalability, and then give you our concrete recommendation with a phased roadmap."

---

## Slide 3 — Client Context

**Who is Nasamotor?**
- Leading automotive dealership group in Portugal
- Managing multiple brands, dealerships, and business lines
- Current core system: DMS (Dealer Management System)
- Reporting: Decentralized, user-driven, Power BI ad hoc

**The Challenge:**
> Business users are building reports independently using DMS extracts — creating inconsistency, governance gaps, and a lack of centralized standards.

---

**What to say:**  
"Let me set the scene. Nasamotor operates a complex business: multiple brands, multiple locations, and a wide range of teams — sales, finance, operations, and management — each needing data to make decisions. Currently, the main source of truth is the DMS system, but reporting is entirely decentralized. People are pulling their own extracts and building their own Power BI files. This creates a fragmented picture of the business."

---

## Slide 4 — Current Pain Points

**What's broken today:**

| Pain Point | Business Impact |
|---|---|
| Inconsistent KPIs across teams | Conflicting data in management meetings |
| No single source of truth | Distrust in reported numbers |
| No governance on data access | Risk of sensitive data exposure |
| Ad hoc reports, no lifecycle | Huge duplication of effort |
| Dependency on individual knowledge | Key-person risk |
| No audit trail on report usage | Compliance exposure |

---

**What to say:**  
"When we dug into the current state with the team, six core pain points emerged. The most critical is the lack of a single source of truth — teams are working from different numbers. This means management decisions are being made on inconsistent data. Beyond accuracy, there are governance and compliance risks when sensitive commercial or financial data is accessible without controls. And from an efficiency standpoint, every department is rebuilding the same reports from scratch."

---

## Slide 5 — The Target Vision

**What Nasamotor needs:**

```
ONE source of truth
        ↓
Governed data layer (who sees what)
        ↓
Certified, centralized Power BI models
        ↓
Self-service reporting with guardrails
        ↓
Scalable across brands, sites, geographies
```

**Success Criteria:**
- 100% of KPIs have agreed business definitions
- Role-based data access enforced by policy
- Report creation time reduced by ≥60%
- Business users empowered, not dependent on IT

---

**What to say:**  
"Our target vision is a layered architecture. It starts with data — getting all the right data from the DMS and other sources into one trusted, governed data store. On top of that, we build certified Power BI models with agreed definitions. Business users then self-serve within defined guardrails. And the whole thing scales as Nasamotor grows. We've defined four measurable success criteria to track whether we've actually solved the problem."

---

## Slide 6 — Two Options Explored

**Option 1: Standard Data & BI Approach**
> Build a data lake → Establish governance → Centralized Power BI framework → Role-based access

**Option 2: AI-Driven Reporting Approach**
> All of Option 1 + AI layer for natural language querying, automated insights, and conversational analytics

**Both options share a common data foundation.**  
Option 2 extends Option 1 with AI capabilities.

---

**What to say:**  
"We evaluated two strategic options. Option 1 is a best-practice, proven BI architecture — build a data lake, add a governance layer, and create a centralized Power BI framework. Option 2 takes all of that and adds AI capabilities on top — things like asking your data questions in plain English, automated anomaly detection, and AI-generated summaries. Importantly, Option 2 requires Option 1 as its foundation — you can't have AI-driven insights without a clean, governed data layer."

---

## Slide 7 — Option 1: Architecture Overview

**Standard BI & Data Approach**

```
[DMS] [CRM] [ERP] [Finance] [HR]
              ↓
       DATA LAKE / LAKEHOUSE
     (Azure Synapse / Databricks)
     Bronze → Silver → Gold layers
              ↓
      DATA GOVERNANCE LAYER
    (Microsoft Purview / Collibra)
    Catalog | Lineage | Classification
              ↓
     POWER BI FRAMEWORK
    Certified datasets | RLS | Templates
              ↓
    [Sales Team] [Finance] [Management] [Ops]
```

---

**What to say:**  
"Let me walk you through the architecture of Option 1. At the bottom, we have the source systems — DMS, CRM, ERP, and any other operational tools. We ingest data from all of these into a cloud-based data lake, structured in three quality layers: raw data, cleaned data, and business-ready data. Above that sits the governance layer — this is where we define who can see what, what data means, and where it came from. At the top, Power BI connects to certified, trusted datasets, and business users can build reports within defined standards."

---

## Slide 8 — Option 1: Key Components

**Building Blocks:**

| Component | Technology Options |
|---|---|
| Data Ingestion | Azure Data Factory, Fivetran, Airbyte |
| Data Lake Storage | Azure ADLS Gen2, Databricks Delta Lake |
| Transformation | dbt, Azure Synapse Pipelines |
| Governance | Microsoft Purview, Collibra |
| Reporting Layer | Power BI Premium, Paginated Reports |
| Access Control | Azure Active Directory, Row-Level Security |

---

**What to say:**  
"These are the specific technologies we recommend for each layer. Nasamotor is likely already in the Microsoft ecosystem given DMS and Office 365 usage, so we've prioritized Azure-native services — Azure Data Factory for ingestion, Azure Data Lake for storage, Microsoft Purview for governance, and Power BI Premium for the reporting layer. This gives us a fully integrated, enterprise-grade stack with strong vendor support and a manageable learning curve."

---

## Slide 9 — Option 1: Pros & Cons

| ✅ Pros | ❌ Cons |
|---|---|
| Proven, battle-tested technology | High upfront infrastructure cost |
| Enterprise-grade governance & security | Long build time: 6–12 months |
| Rich Power BI visualization ecosystem | Requires data engineering expertise |
| Strong vendor support (Microsoft) | Business users still need Power BI training |
| Fully auditable data lineage | Change management effort required |
| Can evolve to Option 2 later | Limited self-service for non-technical users |

---

**What to say:**  
"Option 1 is a solid, proven approach. The pros are clear: it's enterprise-grade, it solves all the governance pain points, and it gives us a future-proof foundation. The cons are mainly time and cost — this is not a quick win. It requires a data engineering team, a realistic 6-to-12 month timeline, and investment in training. These are manageable risks, but they need to be planned for."

---

## Slide 10 — Option 2: AI Layer Overview

**AI-Driven Reporting Approach**

```
              [Option 1 Foundation]
                       ↓
            AI CAPABILITIES LAYER
    ┌──────────────────────────────────────┐
    │  Natural Language Querying (NLQ)     │
    │  → Power BI Q&A + Azure OpenAI       │
    │                                      │
    │  Automated Insight Summaries         │
    │  → AI narratives on dashboards       │
    │                                      │
    │  Anomaly Detection & Alerts          │
    │  → ML models on KPIs                 │
    │                                      │
    │  Conversational Analytics (RAG)      │
    │  → "Ask your data" chatbot           │
    └──────────────────────────────────────┘
                       ↓
         [Any User, Any Device, Plain English]
```

---

**What to say:**  
"Option 2 takes everything from Option 1 and adds an AI intelligence layer on top. The most exciting capability is natural language querying — business users can literally type a question like 'What were the top-selling models last month in Lisbon?' and the AI interprets that question, queries the data, and returns an answer. We also get automated summaries — the system can narrate what's happening in the numbers, flag anomalies before humans notice, and push proactive insights to the right people."

---

## Slide 11 — Option 2: AI Capabilities Deep Dive

**Four AI Capabilities Explained:**

1. **Natural Language Querying (NLQ)**  
   → Business users ask questions in plain language. No Power BI skills needed.

2. **Auto-Generated Insights**  
   → AI writes the "story" behind the numbers automatically.

3. **Anomaly Detection**  
   → ML flags when a KPI deviates from expected range and alerts the right person.

4. **Conversational Analytics (RAG)**  
   → A chatbot grounded in Nasamotor's own data answers complex questions with cited sources.

---

**What to say:**  
"Let me unpack the four AI capabilities. First, NLQ — this is the most impactful for business adoption because it removes the barrier of Power BI expertise. Second, auto-generated insights mean a sales manager gets a morning briefing that says 'Lead volume is up 12% week-on-week but conversion is down 3% — here's why.' Third, anomaly detection — instead of humans reviewing 50 KPIs every day, the system watches all of them and only pings you when something needs attention. Fourth, conversational analytics — think of it as ChatGPT, but trained exclusively on Nasamotor's data, with zero hallucinations on invented facts."

---

## Slide 12 — Option 2: Pros & Cons

| ✅ Pros | ❌ Cons |
|---|---|
| Reduces dependency on Power BI expertise | Significantly higher complexity |
| Business users access insights via chat/NLQ | LLM hallucination risk on business data |
| Faster insight discovery | Requires near-perfect data quality as input |
| Auto anomaly detection saves analyst time | Higher ongoing AI infrastructure cost |
| Future-ready — AI-native architecture | AI governance & prompt guardrails needed |
| Competitive differentiation for Nasamotor | Intensive change management required |

---

**What to say:**  
"Option 2's pros are compelling — especially for business adoption. The more accessible insights are, the more people use data to make decisions. But the cons are real. AI systems can produce wrong answers — this is called hallucination — and in a business context, a wrong revenue number could cause serious problems. That's why data quality must be airtight before deploying AI on top. The good news is that if we build Option 1 properly, Option 2 becomes a natural and safe extension."

---

## Slide 13 — Financial Analysis

**Cost Comparison:**

| Cost Dimension | Option 1 | Option 2 |
|---|---|---|
| Initial Build Cost | €80k–€150k | €110k–€210k |
| Cloud Infrastructure/month | €3k–€8k | €5k–€15k |
| Power BI Premium/month | ~€5k | ~€5k |
| AI Services/month | — | €2k–€8k |
| Training & Change Mgmt | €10k–€20k | €15k–€30k |
| Annual Maintenance | €25k–€50k | €35k–€70k |
| **Estimated Year 1 Total** | **€180k–€280k** | **€240k–€380k** |
| **ROI Timeframe** | **18–24 months** | **24–36 months** |

---

**What to say:**  
"Let's talk money. Option 1 is a substantial investment but within normal range for an enterprise BI transformation — we're looking at €180k to €280k in year 1 including build, infrastructure, licenses, and training. Option 2 adds a 30–40% premium, mainly from AI infrastructure and additional change management. The ROI timeline is longer for Option 2, but the long-term savings from reduced report-building effort and faster decision-making are significant. The exact figures will depend on the final scope and technology choices — these are directional estimates."

---

## Slide 14 — Maintenance Implications

**What ongoing maintenance looks like:**

**Option 1:**
- Monitor data pipelines daily
- Update data models when DMS structure changes
- Manage Power BI report lifecycle (retire old reports)
- Maintain governance policies and access rights
- Monthly performance review

**Option 2 (in addition to Option 1):**
- LLM prompt versioning & tuning
- AI output quality monitoring
- Model retraining / fine-tuning cycles
- Governance of AI-generated content

**Recommended team:**
- 1x Data Engineer (full-time)
- 1x BI Developer / Analyst
- 0.5x AI/ML Engineer (for Option 2)

---

**What to say:**  
"Maintenance is often underestimated in BI projects. Option 1 requires a small but dedicated team — primarily a data engineer and a BI developer. Option 2 adds an AI/ML engineer, at least part-time, to maintain the AI layer. The key maintenance tasks are keeping pipelines healthy, updating models when source systems change, and managing the governance policies. For Option 2, you also need to validate AI outputs regularly — this is non-negotiable to maintain trust in the system."

---

## Slide 15 — Scalability Analysis

**How each option scales:**

| Scalability Dimension | Option 1 | Option 2 |
|---|---|---|
| New data sources | Add pipeline, minimal effort | Same as Option 1 |
| New business units / brands | Configure access roles | Same + retrain NLQ context |
| More users | Scale Power BI capacity tier | Scale AI API limits |
| New KPIs / reports | Add to certified dataset | NLQ handles automatically |
| Multi-region / multi-language | Requires localisation effort | AI supports multiple languages natively |
| Volume of data | Cloud scales elastically | Cloud scales elastically |

**Verdict:** Both options are cloud-native and scale well.  
Option 2 has an edge in user scalability — adding users doesn't mean adding report development capacity.

---

**What to say:**  
"Both options are built on cloud-native infrastructure, so they scale elastically — if Nasamotor grows, the infrastructure grows with it. The key scalability advantage of Option 2 is on the user side: in Option 1, if you have 50 more users wanting custom reports, you need more BI developers. In Option 2, those 50 users just ask their questions in natural language — no additional development needed. That's a meaningful operational advantage at scale."

---

## Slide 16 — Risk Assessment

**Key Risks & Mitigations:**

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| Data quality issues delay delivery | High | High | Start with data audit in Week 1 |
| DMS API limitations for integration | Medium | High | Early technical assessment |
| User adoption resistance | Medium | Medium | Training & change management plan |
| LLM hallucination (Option 2) | Medium | High | Human-in-the-loop validation |
| Budget overrun | Medium | Medium | Phased delivery with clear milestones |
| Vendor lock-in | Low | Medium | Open standards & documented architecture |

---

**What to say:**  
"No transformation is risk-free. The two biggest risks are data quality — if the underlying data is dirty, neither option will deliver accurate insights — and for Option 2 specifically, AI hallucination. We've mapped out mitigations for each risk. The most important action is starting with a data audit before anything else. This tells us how much cleansing work is needed and de-risks the entire project."

---

## Slide 17 — Recommendation

**Our Recommendation: Phased Approach**

```
PHASE 1 (Months 1–6): Option 1 Foundation
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
✅ Build Azure Data Lake (Bronze/Silver/Gold)
✅ Connect DMS + 2 additional sources
✅ Implement Microsoft Purview governance
✅ Create 5 certified Power BI dashboards
✅ Deploy role-based access (RBAC)
✅ Train Power BI Champions per department

PHASE 2 (Months 7–18): Option 2 AI Layer
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🤖 Enable Power BI Q&A on certified datasets
🤖 Deploy Azure OpenAI for NLQ
🤖 Build conversational analytics chatbot
🤖 Implement anomaly detection on top 10 KPIs
🤖 Auto-narrative dashboards for management
```

---

**What to say:**  
"Our recommendation is a phased approach. Don't try to boil the ocean on day one. In Phase 1, we build the data foundation right — data lake, governance, and a certified Power BI framework. This alone solves the biggest pain points: inconsistency and governance. In Phase 2, once the data is clean and trusted, we overlay the AI capabilities. This phased approach reduces risk, delivers early value, and ensures the AI layer is built on solid ground."

---

## Slide 18 — Roadmap

**18-Month Delivery Roadmap:**

| Month | Milestone |
|---|---|
| 1–2 | Data audit, DMS API assessment, architecture design |
| 3–4 | Data lake build, DMS ingestion pipeline live |
| 5–6 | Governance layer deployed, first certified Power BI datasets |
| 7–8 | 5 departmental dashboards live, RBAC enforced, training done |
| 9–10 | AI Phase kickoff — NLQ & Q&A enabled on datasets |
| 11–13 | Conversational analytics chatbot deployed (internal pilot) |
| 14–16 | Anomaly detection live, auto-narrative dashboards |
| 17–18 | Full AI layer rollout, hypercare & optimization |

---

**What to say:**  
"This is our 18-month roadmap broken down into concrete milestones. We've structured it so that there is business value delivered by Month 8 — departments have live, governed dashboards — even before the AI phase starts. This is intentional: it builds trust in the system, gets users engaged, and ensures Phase 2 is built on validated, high-quality data."

---

## Slide 19 — Success Metrics (KPIs for the Project)

**How we'll measure success:**

| Metric | Baseline (Today) | Target (Month 18) |
|---|---|---|
| Reports using certified datasets | ~5% | ≥80% |
| Time to create new business report | 3–5 days | <4 hours |
| Number of governed KPI definitions | 0 | ≥50 |
| Data access incidents | Unknown | 0 |
| Management satisfaction with data | Low | High (survey) |
| AI query usage (Option 2) | 0 | ≥50 queries/day |

---

**What to say:**  
"We believe that what gets measured gets managed. So we've defined six concrete metrics to track whether this transformation is working. The most powerful one is: what percentage of reports use certified, governed datasets? Today it's essentially zero. By month 18, we want it to be 80% or higher. That tells us whether people trust and use the central platform — which is the real measure of success."

---

## Slide 20 — Next Steps

**Immediate Actions:**

| Action | Owner | Timeline |
|---|---|---|
| Approve project scope and budget | Nasamotor Leadership | Week 1–2 |
| Assign internal project sponsor | Nasamotor | Week 1 |
| Conduct DMS API and data quality audit | Joint team | Weeks 2–4 |
| Finalize technology selection | Sycorax / Nasamotor IT | Week 3 |
| Kick off Phase 1 — Data Lake Design | Project team | Week 4 |
| Schedule Phase 1 governance workshop | Project manager | Week 2 |

---

**Thank you.**

*Questions & Discussion*

*Contact: [Ahmed & Paulo — Sycorax Team]*

---

**What to say:**  
"To close, here are the six actions we need to move forward. The most critical is alignment on scope and budget — that needs to happen in the next two weeks. At the same time, we'll get started on the data audit, which is a low-cost, high-value activity that de-risks everything that comes after. We're excited about this journey with Nasamotor and confident that with the right foundation, we can transform how your teams access and use data. Thank you — we're happy to take questions."
