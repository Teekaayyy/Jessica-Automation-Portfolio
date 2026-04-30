# n8n Automation Portfolio

A collection of 40 production-ready n8n workflow automations spanning CRM, AI, data engineering, lead generation, and analytics. Each workflow is fully documented with node-by-node breakdowns, setup instructions, and importable JSON files.

---

## 🔗 Live Portfolio

View the full interactive portfolio with workflow screenshots, node documentation, and downloadable JSONs at 🌐 [Portfolio Website](https://jessica-automation.netlify.app/).

---

## 📁 Repository Structure

```
portfolio-v3.html          # Main portfolio site (single-file, no dependencies)
workflow-01-*.json         # Importable n8n workflow files
workflow-02-*.json
...
workflow-40-*.json
README.md
```

---

## 🤖 Workflows (1–40)

| # | Workflow | Category | Nodes |
|---|----------|----------|-------|
| 01 | Lead Intelligence Pipeline | CRM, Lead Gen | 6 |
| 02 | Automated KPI Report Generator | Analytics, AI | 6 |
| 03 | CRM Deal Stage Automator | CRM, AI | 5 |
| 04 | Customer Health Score Engine | CRM, Analytics | 6 |
| 05 | Social Listening → CRM Sync | CRM, Analytics | 6 |
| 06 | Data Annotation Workflow | Data, AI | 7 |
| 07 | Competitor Price Monitor | Analytics, Data | 9 |
| 08 | Meeting Notes → CRM Sync | CRM, AI | 6 |
| 09 | ETL Pipeline: API → Database | Data, Analytics | 7 |
| 10 | Survey Analysis Engine | Analytics, AI, CRM | 9 |
| 11 | LinkedIn Prospect → CRM Pipeline | CRM, Lead Gen | 6 |
| 12 | Churn Prediction Alert System | CRM, Analytics | 7 |
| 13 | Support Ticket Enrichment & Router | CRM, AI | 10 |
| 14 | Automated Follow-up Sequencer | CRM | 8 |
| 15 | Data Deduplication Engine | Data, Analytics | 8 |
| 16 | Sales Call Sentiment Analyzer | CRM, AI, Analytics | 9 |
| 17 | Contract Renewal Pipeline | CRM | 9 |
| 18 | Real-time Dashboard Updater | Analytics, Data | 9 |
| 19 | AI Data Labeling Pipeline | Data, AI | 9 |
| 20 | Customer Onboarding Orchestrator | CRM, Analytics | 15 |
| 21 | AI Lead Scoring Engine | CRM, AI, Analytics | 8 |
| 22 | Competitive Intelligence Automation | Analytics, AI, Data | 9 |
| 23 | Multi-Touch Revenue Attribution | Analytics, Data, CRM | 8 |
| 24 | AI Personalised Email Campaign Engine | CRM, AI, Lead Gen | 9 |
| 25 | SLA Breach Monitor & Escalation | CRM, AI | 7 |
| 26 | Behavioral Segmentation CRM Sync | Analytics, Data, CRM | 7 |
| 27 | AI Contract Intelligence Pipeline | AI, Data, CRM | 8 |
| 28 | Hiring Signal Outreach Pipeline | Lead Gen, AI, CRM | 8 |
| 29 | Multi-Channel Churn Intervention | CRM, AI, Analytics | 10 |
| 30 | RevOps Intelligence Dashboard | Analytics, Data | 10 |
| 31 | Voice of Customer Intelligence Engine | Analytics, AI, Data | 9 |
| 32 | Sales Call Intelligence & Coaching Engine | CRM, AI, Analytics | 8 |
| 33 | Revenue Expansion & Upsell Engine | CRM, AI, Analytics | 8 |
| 34 | Automated SEO Content Intelligence | Analytics, AI, Data | 8 |
| 35 | Financial Reconciliation & Discrepancy Engine | Data, Analytics | 8 |
| 36 | Customer Journey Milestone Orchestrator | CRM, Analytics | 9 |
| 37 | AI Talent Market Intelligence Pipeline | Analytics, AI, Data | 8 |
| 38 | Partner Performance Intelligence System | CRM, Analytics, Data | 9 |
| 39 | AI Product Feedback to Roadmap Pipeline | AI, Data, CRM | 9 |
| 40 | Automated Board & Investor Reporting Engine | Analytics, AI, Data | 10 |

---

## 🛠️ Tech Stack

- **Automation** — n8n (self-hosted or cloud)
- **AI** — OpenAI GPT-4o / GPT-4o-mini
- **CRM** — HubSpot
- **Data** — PostgreSQL, Google Sheets, Airtable
- **Comms** — Gmail, Slack
- **Analytics** — Google Analytics 4 (GA4)
- **Payments** — Stripe
- **Transcription** — AssemblyAI
- **Prospecting** — Phantombuster, Apollo.io

---

## 🚀 How to Import a Workflow

1. Open your n8n instance
2. Click **Workflows → New Workflow**
3. Click the **⋯ menu → Import from File**
4. Select the relevant `workflow-XX-*.json` file
5. Replace all `REPLACE_WITH_YOUR_CREDENTIAL_ID` placeholders with your actual n8n credentials
6. Update any environment variables listed in the sticky note inside the workflow
7. Set the workflow to **Active** when ready

> All workflows are imported with `active: false` by default — they will not run until you explicitly activate them.

---

## ⚙️ Environment Variables

Most workflows rely on n8n environment variables rather than hardcoded values. Common variables across the collection:

| Variable | Used In |
|----------|---------|
| `HUBSPOT_API_TOKEN` | Multiple workflows |
| `OPENAI_API_KEY` | All AI workflows |
| `ASSEMBLYAI_API_KEY` | Workflow 16 |
| `PHANTOMBUSTER_API_KEY` | Workflow 11 |
| `PHANTOMBUSTER_AGENT_ID` | Workflow 11 |
| `APOLLO_API_KEY` | Multiple workflows |
| `STRIPE_SECRET_KEY` | Workflow 18 |
| `SLACK_WEBHOOK_URL` | Multiple workflows |
| `REP_NAME` | Workflow 14 |
| `PRODUCT_NAME` | Workflow 20 |
| `COMPETITOR_A_URL` | Workflow 07 |

Set these in n8n under **Settings → Environment Variables**.

---

## 📋 Workflow Highlights

**Workflow 12 — Churn Prediction Alert System**
Runs every Sunday night. Pulls 90 days of product usage data from PostgreSQL, scores each account across four weighted signals (login frequency, feature breadth, recency, support volume), updates HubSpot with the churn risk level, and sends a personal re-engagement email for high-risk accounts before the CS team starts Monday morning.

**Workflow 13 — Support Ticket Enrichment & Router**
Every incoming ticket is enriched with the customer's HubSpot context (plan, health score, lifecycle stage) before AI triage. GPT-4o-mini classifies category and priority accounting for customer tier, then routes to one of four dedicated Slack channels — all within seconds of ticket submission.

**Workflow 18 — Real-time Dashboard Updater**
Pulls from HubSpot, GA4, and Stripe in parallel every 15 minutes and aggregates pipeline value, web sessions, conversions, and daily revenue into a single Google Sheets row. Connect Looker Studio or Metabase to the sheet for a live business dashboard with no manual data entry.

**Workflow 20 — Customer Onboarding Orchestrator**
Triggers when a contact becomes a customer in HubSpot. Sends a Day 0 welcome email immediately, waits 3 days, checks milestone completion from PostgreSQL, then routes to a celebration email (2+ milestones complete) or a nudge email (behind schedule). VIP accounts (deal value ≥ £5,000) get an additional Slack alert to the CS team.

**Workflow 29 — Multi-Channel Churn Intervention**
When a churn score threshold is crossed, fires a coordinated 10-day retention sequence automatically: Day 0 CSM email, Day 2 in-app banner, Day 5 executive call invite, Day 10 personalised retention offer — every touchpoint logged back to HubSpot throughout.

**Workflow 32 — Sales Call Intelligence & Coaching Engine**
Triggered by a transcript webhook, the workflow scores each sales call across 8 methodology dimensions, generates personalised coaching notes for the rep, logs everything to HubSpot, and compiles a weekly performance digest — turning every call into a coaching opportunity with zero manual review.

**Workflow 35 — Financial Reconciliation & Discrepancy Engine**
Runs daily across Stripe, HubSpot, and Xero — cross-referencing all three with four reconciliation checks, classifying any discrepancies by severity, and delivering a structured report with Slack alerts for critical items. Finance gets eyes on problems before they become month-end surprises.

**Workflow 39 — AI Product Feedback to Roadmap Pipeline**
Aggregates feedback weekly from four sources, uses AI to cluster it into feature themes, then scores each theme by ARR impact and submission frequency. Themes that cross the prioritisation threshold automatically become Jira epics — closing the loop between customer voice and the product roadmap.

---

## 📄 Licence

These workflows are shared for portfolio and educational purposes. Feel free to adapt them for your own use. Attribution appreciated but not required.

---

## 👤 Author

**Jessica Dan-Odhomo**
Automation Engineer · Data Analyst · Mechatronics Engineer

- 🌐 [Portfolio Website](https://jessica-automation.netlify.app/)
- 🔗 [linkedin.com/in/jessica-dan-odhomo](https://www.linkedin.com/in/jessica-dan-odhomo)
- 📧 jessicatekome@gmail.com
