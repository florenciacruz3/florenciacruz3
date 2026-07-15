# The Hidden Risks in Your Microsoft Fabric Tenant — and How to Find Them Before They Find You

---

## Overview

**Who this article is for:**

This article is intended for enterprise teams managing 50+ workspaces and planning a move to Fabric.

**What you will learn** — click any section to jump directly to it:

1. [What Microsoft Fabric Is and Why Your Tenant Matters](#1-what-microsoft-fabric-is-and-why-your-tenant-matters)
2. [How It Works](#2-how-it-works)
3. [Who It Is For](#3-who-it-is-for)
4. [What You Get](#4-what-you-get)
5. [Expected Outcomes](#5-expected-outcomes)
6. [Assessment Tiers](#6-assessment-tiers)
7. [Get Started](#7-get-started)

**What this article does *not* cover:**

- How to perform a tenant audit manually
- Microsoft Fabric setup 
- Advanced Fabric architecture concepts

> ⏱ Estimated reading time: 9 minutes

---

## 1. What Microsoft Fabric Is and Why Your Tenant Matters

There is a moment every data leader fears. The Microsoft Fabric migration is approved, the timeline is set, and then the project fails.

Here is why that happens: 

Companies let their data environments get messy over years, and when they try to move to Fabric, the mess slows everything down or causes costly surprises.

Specifically, three things go wrong in almost every large company:
1.	Teams create workspaces and forget about them (sprawl).
2.	People leave the company but their access to data does not get removed (orphaned access — this is a security risk).
3.	The company keeps paying for software licenses for people who no longer use them (waste).

Tenant Scan finds all of this before the migration happens, so companies are not discovering it mid-move.

Microsoft Fabric is an all-in-one data platform — a single 
environment where data is stored, organized, analyzed, and 
turned into reports. At the center of every Fabric deployment 
is your tenant — your organization's private corner of 
Microsoft's cloud, where every workspace, dataset, report, 
and permission lives.

Without regular governance, that environment accumulates 
problems that remain unnoticed until you decide to migrate.

---

## 2. How It Works

During a tenant scan the environment that your data moves through goes through a specific read-only assessment of your Fabric and Power BI environment. Nothing in your tenant is modified

The assessment examines ten governance failure points that 
consistently block or complicate Fabric migrations:

1. **Capacity governance** — whether compute resources are 
   correctly sized and allocated
2. **Workspace sprawl and lifecycle** — locating all unowned, 
   inactive, or redundant workspaces accumulating over time
3. **OneLake security** — whether row-level and column-level 
   security configurations across lakehouses and datasets 
   are set up correctly
4. **Sensitivity labels and Data Loss Prevention (DLP)** — whether sensitive data 
   is classified and protected according to your 
   organization's policies
5. **Semantic model hygiene** — checking for duplicated or 
   undocumented models creating reporting inconsistencies
6. **Data lineage** — tracing where data comes from and how 
   it flows through the environment
7. **Identity and connections** — finding service accounts 
   and access permissions that have drifted from their 
   original intent
8. **Domains** — whether workspaces and assets are correctly 
   organized and governed by domain
9. **Deployment and source control** — whether pipelines and 
   reports are version-controlled and deployed consistently
10. **Monitoring and cost accountability** — whether usage, 
    performance, and spend are visible and assigned to owners

**The process:**

1. **Intake** — complete a structured questionnaire covering 
   your environment and migration goals
2. **Scan** — PowerMates performs a read-only enumeration of 
   your tenant, at the depth your tier allows
3. **Report** — receive your scored Fabric Readiness Report 
   in 3–5 business days

Tenant Scan examines this entire environment — identifying accumulated problems that will slow down or block a migration.

---

## 3. Who It Is For

Tenant Scan is designed for you if you are:

- Planning a migration to Microsoft Fabric and need to know 
  what is in your current environment before you commit
  
- Managing 50 or more workspaces or datasets in an existing 
  Power BI tenant
  
- Tired of paying for licenses assigned to inactive users 
  and want to identify where budget is being wasted
  
- About to start a migration and cannot afford to discover 
  problems halfway through

---

## 4. What You Get

Every Tenant Scan engagement delivers three outputs:

- **Executive Summary with RAG Rating** — a Red, Amber, and 
Green (RAG) status that gives leadership an immediate read on 
  migration readiness without requiring technical context.

- **10-Point Governance Scorecard** — findings across all ten governance failure points, ranked by impact and effort.
  
- **Now, Next, and Later Remediation Roadmap** — a structured 
  action plan that sequences your top findings into an 
  executable 90-day window, rather than an overwhelming 
  backlog.

> [!NOTE]
> The entire intake process runs through a structured 
> 15-minute questionnaire. Tenant access — where required 
> by tier — is read-only and used solely for assessment 
> purposes. Nothing in your environment is modified.

Tenant Scan is the first step in a four-stage path:

1. Tenant Scan
2. Architecture
3. Build
4. Govern

Organizations that complete the scan leave with a clear 
picture of where they stand and a defined path to where 
they need to be.

---

## 5. Expected Outcomes

> [!NOTE]
> The scenarios below are illustrative — representative of 
> what engagements at this scale typically surface based on 
> the governance failure points Tenant Scan examines.

- **30-day remediation** — A retail organization with 200+ 
  workspaces is expected to surface overshared datasets and workspaces 
  with no assigned owner. With a ranked action plan in hand, 
  the team will resolve the highest-impact findings within 
  a month.

- **Significant license savings** — A financial services 
  organization could potentially identify unused licenses and underutilized 
  Premium capacity that had been draining budget undetected 
  — costs that would be invisible without a structured audit.

- **Migration-ready in one quarter** — A healthcare 
  organization with 400 workspaces could receive a scored 
  readiness report and a phased roadmap. With clear 
  priorities and a sequenced plan, the first workspaces 
  is predicted to go live in Fabric within the quarter.

---

## 6. Assessment Tiers

Tenant Scan is available at three levels. The tier you choose 
determines the depth of the assessment and the level of detail 
in your results.

*Table: Comparison of three Tenant Scan assessment tiers — 
Starter at $2,500, Professional at $5,000, and Enterprise 
at $7,500 — showing price and what is included at each level.*

| Tier | Price | What It Includes |
|---|---|---|
| **Starter** | $2,500 | Intake through a 15-minute questionnaire. Executive summary, 10-point scorecard, and Now, Next, and Later roadmap delivered in 3–5 business days. No tenant access required. |
| **Professional** | $5,000 | Everything in Starter, plus a deeper read-only enumeration of your tenant via the Fabric Command Line Interface (CLI) for more detailed findings across all ten governance failure points. |
| **Enterprise** | $7,500 | Everything in Professional, with the most comprehensive scope — full environment coverage for organizations with the most complex or large-scale tenant environments. |

> [!TIP]
> No tenant is modified at any stage of the process.
> Tenant access in the Professional and Enterprise tiers 
> is read-only and used solely for assessment purposes.

---

## 7. Get Started

Most organizations discover governance gaps when it is 
already too late.

The Tenant Scan gives you the map before you move.

The problems are knowable. The question is whether you find 
them before they find you.

**Pick a tier. Complete the questionnaire. Get your scored 
Fabric Readiness Report in 3–5 business days.**

[Start your Tenant Scan assessment at PowerMates](https://www.thepowermates.com/tenant-scan)

---

## About PowerMates

Founded by two Microsoft Most Valuable Professionals (MVPs) with over 20 years of combined experience in this area, PowerMates is an enterprise consulting firm that focuses on Microsoft data and AI platforms to help organizations reduce governance risk, accelerate AI adoption, and avoid unnecessary costly missteps when migrating to Microsoft Fabric. 

PowerMates operates across three core areas: 

- **Consulting** — Eight specialized service offerings, ranging from governance audits to full architecture design and migration support. 

- **Content** — Deep-dive videos and technical walkthroughs covering Fabric governance, migration strategy, and AI adoption, published across YouTube, LinkedIn, TikTok, and other platforms to help enterprise teams make faster, more informed infrastructure decisions.

- **Community** — Conference speaking engagements, open-source tooling, and ongoing knowledge-sharing with the broader Microsoft data community, built on the belief that expertise should scale through accessible, honest content.

The company has built a following of 7,300+ subscribers on YouTube and maintains an active presence across major social platforms, positioning itself as a practitioner-led voice in the Fabric governance and enterprise AI space.

---

## FAQ

### Does PowerMates need access to our tenant to run a scan?

It depends. Tenant Scan does not require any tenant access if you choose the starter tier. The entire intake process will run through a 15-minute questionnaire only. The two next tiers, professional and enterprise do require looking at your tenant in order to run a scan. In all cases, nothing in your tenant is written to or 
modified at any stage. 

---

### How disruptive is this to our team?

Minimal. Beyond the initial 15-minute questionnaire, your team 
will not need to be pulled off their regular work. This does not require ongoing internal involvement.

---

### What if we already think we know what's in our tenant?

Problems in the environment happen because most teams underestimate the scope of the problem. Typical findings — 30 to 40 percent workspace sprawl and 25 to 30 percent orphaned access — are discovered 
precisely because teams lack visibility into their own 
environment.

---

### What's the difference between this and Microsoft's built-in admin reporting?

Microsoft's tools report raw data. Tenant Scan turns that data 
into an actionable report — specifically, a ranked top 5 action 
plan built from the findings, rather than a list of numbers with 
no clear next step.

---

### Is this only useful right before a migration?

No. Regardless of whether a migration is planned, workspace sprawl, orphaned access, and license waste are worth identifying for any organization looking to reduce cost and risk. 

---

### What happens after we receive the report?

You receive your Fabric Readiness Score, a full governance and 
license audit, and a prioritized action plan covering your top 5 
recommended actions — each one rated by impact and effort, and 
designed to be executable within 90 days.
