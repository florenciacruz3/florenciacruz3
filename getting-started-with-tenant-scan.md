# Getting Started with Tenant Scan
## The Hidden Risks in Your Microsoft Fabric Tenant — and How to Find Them Before They Find You

---

## Overview

**Who this article is for:**

This article is intended for enterprise teams managing 50+ workspaces and planning a move to Fabric.

**What you will learn:**

1. [What Microsoft Fabric Is and Why Your Tenant Matters](#1-what-microsoft-fabric-is-and-why-your-tenant-matters)
2. [How It Works](#2-how-it-works)
3. [Comparing Fabric to Other Services](#3-comparing-fabric-to-other-services)
4. [Who It Is For](#4-who-it-is-for)
5. [What You Get](#5-what-you-get)
6. [Expected Outcomes](#6-expected-outcomes)
7. [Get Started](#7-get-started)

**What this article does *not* cover:**

- How to perform a tenant audit manually
- Microsoft Fabric setup 
- Advanced Fabric architecture concepts

> ⏱ Estimated reading time: 8 minutes

---

## 1. What Microsoft Fabric Is and Why Your Tenant Matters

There's a moment every data leader fears. The Microsoft Fabric migration is approved, timeline set, and then the project fails.

Here's why that happens: 

Companies let their data environments get messy over years, and when they try to move to Fabric, the mess slows everything down or causes costly surprises.

Specifically, three things go wrong in almost every large company:
1.	Teams create workspaces and forget about them (sprawl).
2.	People leave the company but their access to data doesn't get removed (orphaned access — this is a security risk).
3.	The company keeps paying for software licenses for people who no longer use them (waste).

Tenant Scan finds all of this before the migration happens, so companies aren't discovering it mid-move.

[Microsoft defines Fabric](https://www.microsoft.com/en-us/microsoft-fabric/resources/data-101/what-is-fabric) 
as "a unified, AI-powered data platform to simplify data management 
and analytics — an end-to-end intelligent data platform with a suite 
of cloud services and tools for every data lifecycle stage: ingestion, 
preparation, storage, analysis, and visualization."

What this means is that Microsoft Fabric is an all-in-one data platform, a single workspace where data is stored, organized, analyzed, and turned into reports. 

At the center of Fabric is your tenant — your organization's private corner of Microsoft's cloud. Everything the company has built in Power BI and Fabric lives in there: every workspace, every 
dataset, every report, every permission. Without 
regular governance, that environment accumulates problems that remain unnoticed until you decided to migrate. 

Section 2 maps exactly what lives inside that tenant — and 
how data moves through it from raw source to finished report.

---

## 2. How It Works

During a tenant scan the environment that your data moves through goes through a specific process. Here is how that environment works, from the moment raw data enters the system to the moment a business user reads a report.

- **Raw Data** — Raw data is data in its original state — exactly as it came out of the system — without any processing, cleaning, transformation, or analysis applied to it.
  
- **Data Factory** — The system that ingests raw data from various sources, transforms it (cleaning, reshaping, and standardizing it into a usable format), and delivers it to OneLake.
  
- **OneLake** — OneLake is Microsoft's unified, data storage layer built into Microsoft Fabric. OneLake acts as a single, centralized repository where all data is stored so that different teams and tools can access the same data without duplicating or moving it around.
  
- **Data Warehouse** — A structured storage layer that consolidates data from OneLake into a format optimized for reporting and analysis.
  
- **Semantic Model** — A layer that translates technical data into business-friendly language and structure, making it easier for non-technical users to work with.

- **Power BI** — Power BI is the part of Fabric that turns data into visual reports and dashboards that business users can read and interact with.

- **Business Users** — A business user is anyone in a company who uses data to make decisions but doesn't build or manage the systems that produce that data.

Tenant Scan examines this entire environment — identifying accumulated problems that will slow down or block a migration.

---

## 3. Comparing Fabric to Other Services

- **Microsoft Azure SQL Database** — think of it as a standalone, fully managed relational tool (PaaS) that lives in Microsoft Azure — a broader cloud platform. It exists independently of Fabric. Fabric, by contrast, is a complete data platform that ingests, stores, transforms, analyzes, and visualizes data. Fabric does not contain Azure SQL Database. Instead Fabric can connect to Azure SQL Database as one of many external data sources.
  
- **Microsoft Power BI** — lives inside Fabric as the final step in the pipline. It's in charg of turning data into charts, graphs, and dashboard meant to be read by business users. Once all the data is gathered, clean, and stored, Power BI is what becomes visible. 
  
- **Microsoft Azure** — the broader cloud platform, offering 200+ services for computing, storage, networking, AI, and more. Azure is the cloude that everything runs on. Fabric is a specific data platform that runs on Azure. Fabric is not a replacement for Azure, but a specialized layer built on top of it — one Azure product focused entirely on packaging data tools (ingestion, storage, warehousing, reporting) into a single ready-to-use system, instead of requiring you to stitch Azure services together yourself.

> [!NOTE]
> Azure and Fabric are not competitors or alternatives to each other. They exist at completely different levels.

---

## 4. Who It Is For

Tenant Scan is designed for you if you are:

- Planning a migration to Microsoft Fabric and needs to know 
  what is in your current environment before you commit
  
- Managing 50 or more workspaces or datasets in an existing 
  Power BI tenant
  
- Tired of paying for licenses assigned to inactive users 
  and want to identify where budget is being wasted
  
- About to start a migration and cannot afford to discover 
  problems halfway through

---

## 5. What You Get

- **Fabric Readiness Score** — A single, easy-to-understand rating from 0 to 100 that reflects how prepared your organization is to adopt or scale Microsoft Fabric. The score is calculated across three core dimensions:

  - **Governance** — how well data access, ownership, and security policies are currently managed.
  - **Complexity** —  how many systems, workspaces, and data sources are involved, and how tangled those dependencies are.
  - **Migration Readiness** —  how much work would be required to move existing workloads (like Azure SQL Database or Power BI reports) into Fabric without disruption.

Rather than a vague "you're not ready yet," this gives leadership a percise, quantfiable benchmark, so pro so progress can be tracked over time.

- **Governance and License Audit** — A detailed review of how your Fabric (or Azure) environment is actually being used versus how it's documented or assumed to be used. This includes:

  - **Workspace ownership mapping** — identifying who owns 
    and controls each workspace
  - **Orphaned access** — users with access they 
    no longer need
  - **License waste** — identifying unused licenses costing 
    money without being used
  - **Sensitivity label coverage** — checking whether 
    sensitive data is properly labeled and protected

The result is a clear picture of where governance gaps exist and where cost savings are hiding.

- **Prioritized Action Plan** — Rather than handing you a long list of every possible improvement, this narrows the findings down to your top 5 highest-impact actions, ranked by an impact-to-effort ratio — meaning the actions that deliver the most value for the least amount of work come first. Each action is scoped to be realistically completed within a 90-day window, giving your team a focused, achievable roadmap.
  
> [!NOTE]
> The entire intake process runs through a structured 15-minute questionnaire.

---

## 6. Expected Outcomes

- **30-day remediation** — A mid-market retail company with 200+ 
  workspaces discovered 47 overshared datasets and 12 workspaces 
  with no owner. Everything resolved within a month.

- **$180,000 saved annually** — A financial services firm 
  identified unused licenses and underutilized Premium capacity 
  that had been draining budget undetected.

- **400 workspaces, migration-ready in one quarter** — A 
  healthcare organization received a scored readiness report 
  and a phased roadmap that got their first 50 workspaces 
  live in Fabric within the quarter.

---

## 7. Get Started

Most organizations discover governance gaps when it is already too late.

The Tenant Scan gives you the map before you move.

The problems are knowable. The question is whether you find 
them before they find you.

**Pick a tier. Complete the questionnaire. Get your scored 
Fabric Readiness Report in 3–5 business days.**

[Get Started →](https://www.thepowermates.com/tenant-scan)

---

## About PowerMates

PowerMates is an enterprise consulting firm focused on Microsoft data and AI platforms, helping organizations reduce governance risk, accelerate AI adoption, and avoid costly missteps when scaling Microsoft Fabric.

The company was founded by two Microsoft MVPs with over 20 years of combined experience in Microsoft data and 
AI platforms.

PowerMates operates across three core areas:

- **Consulting** — Delivered directly by practitioners, PowerMates introduces eight specialized Fabric service offerings, ranging from governance audits to full architecture design and migration support. 

- **Content** — Deep-dive videos and technical walkthroughs covering Fabric governance, migration strategy, and AI adoption, published across YouTube, LinkedIn, TikTok, and other platforms to help enterprise teams make faster, more informed infrastructure decisions.

- **Community** — Conference speaking engagements, open-source tooling, and ongoing knowledge-sharing with the broader Microsoft data community, built on the belief that expertise should scale through accessible, honest content.

The company has built a following of 7,300+ subscribers on YouTube and maintains an active presence across major social platforms, positioning itself as a practitioner-led voice in the Fabric governance and enterprise AI space.

---

## FAQ

### Does PowerMates need access to our tenant to run a scan?

No. Tenant Scan does not require any tenant access. The entire 
intake process runs through a 15-minute questionnaire. 
There's no need for external access to your environment.

---

### How disruptive is this to our team?

Minimal. Beyond the initial 15-minute questionnaire, your team 
will not need to be pulled off their regular work. This does not require ongoing internal involvement.

---

### What if we already think we know what's in our tenant?

Most teams underestimate the scope of the problem. The typical findings — 30 to 40 percent workspace sprawl 
and 25 to 30 percent orphaned access — are discovered 
precisely because teams lack visibility into their own 
environment.

---

### What's the difference between this and Microsoft's built-in admin reporting?

Microsoft's tools show raw data — lists of workspaces, 
licenses, and permissions. Tenant Scan turns that raw data into a 
scored, prioritized, actionable report. The value is not the data itself — it is the analysis and 
the ranked top 5 action plan built from it.

---

### Is this only useful right before a migration?

No. Regardless of whether a migration is planned, workspace sprawl, orphaned access, and license waste are worth identifying for any organization looking to reduce cost and risk. 

---

### What happens after we receive the report?

You receive your Fabric Readiness Score, a full governance and 
license audit, and a prioritized action plan covering your top 5 
recommended actions — each one rated by impact and effort, and 
designed to be executable within 90 days.
