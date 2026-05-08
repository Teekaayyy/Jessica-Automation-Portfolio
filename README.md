# n8n Automation Portfolio

A collection of 50 production-ready n8n workflow automations spanning CRM, AI, data engineering, lead generation, analytics, and ElevenLabs voice automation. Each workflow is fully documented with node-by-node breakdowns, setup instructions, and importable JSON files.

---

## 🔗 Live Portfolio

View the full interactive portfolio with workflow screenshots, node documentation, and downloadable JSONs at 🌐 [Portfolio Website](https://jessica-automation.netlify.app/)

---

## 📁 Repository Structure

```
portfolio-v3.html          # Main portfolio site (single-file, no dependencies)
workflow-01-*.json         # Importable n8n workflow files
workflow-02-*.json
...
workflow-50-*.json
README.md
```

---

## 🤖 Workflows (1–50)

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
| 41 | ElevenLabs Voice Clone Campaign Engine | Voice Agents, AI, Analytics | 8 |
| 42 | ElevenLabs Speech-to-Speech Sales Coach | Voice Agents, AI, CRM | 9 |
| 43 | ElevenLabs Automated Podcast Producer | Voice Agents, AI, Data | 10 |
| 44 | ElevenLabs Multilingual Content Localiser | Voice Agents, AI, Data | 8 |
| 45 | ElevenLabs Voice-Powered Phone Agent | Voice Agents, AI, CRM | 11 |
| 46 | ElevenLabs E-Learning Voice Engine | Voice Agents, AI, Data | 9 |
| 47 | ElevenLabs Voice Broadcast System | Voice Agents, AI, CRM | 8 |
| 48 | ElevenLabs Audio Fine-Tuning Pipeline | Voice Agents, AI, Data | 10 |
| 49 | ElevenLabs Content-to-Audio Newsletter | Voice Agents, AI, Analytics | 8 |
| 50 | ElevenLabs Projects API Editorial Engine | Voice Agents, AI, Data | 10 |

---

## 🎙️ ElevenLabs Voice Agent Workflows (41–50)

These workflows leverage the ElevenLabs API — including Voice Cloning, Speech-to-Speech, Projects API, and TTS — to build production-grade voice automation pipelines integrated with n8n.

**Workflow 41 — ElevenLabs Voice Clone Campaign Engine**
Pulls a contact segment from HubSpot, constructs a personalised script per recipient, synthesises it using an ElevenLabs voice clone (stability 0.75, similarity_boost 0.85), and delivers the audio via WhatsApp or email. Achieves 3× response rate improvement over written outreach with zero manual recording.

**Workflow 42 — ElevenLabs Speech-to-Speech Sales Coach**
After each sales call, Whisper transcribes the recording, GPT-4o identifies 3 coaching moments, and ElevenLabs Speech-to-Speech recasts key call excerpts in a professional coach voice. A consolidated audio debrief lands in the rep's Slack DM within 10 minutes of call end — 100% call coverage with zero manager review time.

**Workflow 43 — ElevenLabs Automated Podcast Producer**
Takes a content brief via webhook, generates a full two-host dialogue script with GPT-4o, synthesises each speaker using dedicated ElevenLabs voice clones with individualised audio parameters, stitches a stereo episode with intro/outro music, and publishes directly to Transistor.fm RSS — a complete episode in under 15 minutes.

**Workflow 44 — ElevenLabs Multilingual Content Localiser**
Translates a master script into 5 languages simultaneously using GPT-4o with culture-specific tone instructions, synthesises each translation using ElevenLabs multilingual_v2 with language-matched voice clones, and uploads all locales to S3 in under 20 minutes. Reduces a 6-week localisation process to 20 minutes.

**Workflow 45 — ElevenLabs Voice-Powered Phone Agent**
A 24/7 inbound phone agent built on Twilio + ElevenLabs. Whisper transcribes each caller turn, GPT-4o formulates contextual responses using full conversation history, and ElevenLabs streaming TTS delivers audio with under 2-second response latency. Handles up to 8-turn dialogues and resolves 65% of queries without human transfer.

**Workflow 46 — ElevenLabs E-Learning Voice Engine**
Triggers when a course script is marked ready in Notion, synthesises each module using ElevenLabs with a consistency-optimised instructor voice clone, packages assets in SCORM-compliant naming, and uploads directly to an LMS via API. Reduces course narration from a 2-week studio process to a 2-hour automated run.

**Workflow 47 — ElevenLabs Voice Broadcast System**
Synthesises urgent announcements with an executive voice clone (stability 0.85), initiates concurrent Twilio outbound calls to a segmented contact list, handles live answer vs voicemail routing, and escalates unanswered contacts to SMS after 3 retries — achieving 94% reach rate for critical communications.

**Workflow 48 — ElevenLabs Audio Fine-Tuning Pipeline**
Systematically tests 27 ElevenLabs parameter combinations (stability × similarity_boost × style) for a voice clone, scores each with Azure PESQ/MOS audio quality assessment, ranks all configurations by composite quality score, and outputs the optimal settings with a full report — eliminating manual trial-and-error from voice configuration.

**Workflow 49 — ElevenLabs Content-to-Audio Newsletter**
Publishes twice-weekly automatically: curates top industry articles from NewsAPI and RSS feeds, generates 100-word editorial summaries with GPT-4o in brand voice, synthesises a 10-minute episode with a presenter voice clone, publishes to Spotify and Apple Podcasts via RSS, and sends an HTML email with embedded audio player — zero human production time.

**Workflow 50 — ElevenLabs Projects API Editorial Engine**
Uses the ElevenLabs Projects API (not the standard TTS endpoint) for full-document synthesis with cross-sentence context awareness — producing publisher-quality audiobooks and long-form audio from manuscripts up to 100,000 characters. Outputs M4B format with chapter navigation markers and distributes to Findaway Voices and ACX.

---

## 🛠️ Tech Stack

- **Automation** — n8n (self-hosted or cloud)
- **AI** — OpenAI GPT-4o / GPT-4o-mini, Whisper STT
- **Voice Synthesis** — ElevenLabs (Voice Cloning, Speech-to-Speech, Projects API, TTS)
- **CRM** — HubSpot
- **Data** — PostgreSQL, Google Sheets, Airtable
- **Comms** — Gmail, Slack, Twilio (SMS + Voice + WhatsApp)
- **Analytics** — Google Analytics 4 (GA4)
- **Payments** — Stripe
- **Transcription** — AssemblyAI
- **Prospecting** — Phantombuster, Apollo.io
- **Storage** — AWS S3
- **Podcast Distribution** — Transistor.fm

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
| `ELEVENLABS_API_KEY` | Workflows 41–50 |
| `ELEVENLABS_VOICE_ID` | Workflows 41–50 |
| `ASSEMBLYAI_API_KEY` | Workflow 16 |
| `PHANTOMBUSTER_API_KEY` | Workflow 11 |
| `PHANTOMBUSTER_AGENT_ID` | Workflow 11 |
| `APOLLO_API_KEY` | Multiple workflows |
| `STRIPE_SECRET_KEY` | Workflow 18 |
| `SLACK_WEBHOOK_URL` | Multiple workflows |
| `TWILIO_ACCOUNT_SID` | Workflows 45, 47 |
| `TWILIO_AUTH_TOKEN` | Workflows 45, 47 |
| `AWS_S3_BUCKET` | Workflows 41, 43, 44, 47, 48 |
| `TRANSISTOR_API_KEY` | Workflows 43, 49 |
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

**Workflow 45 — ElevenLabs Voice-Powered Phone Agent**
A 24/7 inbound phone agent built with Twilio + ElevenLabs streaming TTS. Sub-2-second response latency, 8-turn conversation depth, and 65% query resolution without human transfer — indistinguishable from a live receptionist on standard phone audio.

**Workflow 48 — ElevenLabs Audio Fine-Tuning Pipeline**
The only systematic approach to ElevenLabs voice configuration in the collection. Tests 27 parameter combinations, scores each with PESQ/MOS audio quality metrics, and produces a deployment-ready configuration report — replacing subjective guesswork with objective quality measurement.

---

## 📄 Licence

These workflows are shared for portfolio and educational purposes. Feel free to adapt them for your own use. Attribution appreciated but not required.

---

## 👤 Author

**Jessica Dan-Odhomo**
AI Automation Engineer · Data Analyst · Mechatronics Engineer

- 🌐 [Portfolio Website](https://jessica-automation.netlify.app/)
- 🔗 [linkedin.com/in/jessica-dan-odhomo](https://www.linkedin.com/in/jessica-dan-odhomo)
- 📧 jessicatekome@gmail.com
