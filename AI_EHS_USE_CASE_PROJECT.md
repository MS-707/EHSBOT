# AI in EHS: Digital SDS Portal Use Case

## Project Summary for Claude Cowork

This document outlines a completed workplace improvement project that demonstrates the practical application of AI tools (Claude Cowork and Claude Code) in Environmental Health & Safety (EHS) compliance. Use this as a template for building a business case for enterprise AI adoption.

---

## Executive Summary

**Project:** Digital Safety Data Sheet (SDS) Portal
**Live URL:** https://ehsbot.vercel.app/
**Chemicals Indexed:** 73
**Development Time:** ~8 hours (vs. 25-36 hours traditional approach)
**Ongoing Cost:** $0/year
**Compliance Standards Met:** OSHA 29 CFR 1910.1200, Cal/OSHA Title 8 Section 5194

### The Problem Solved

Hazard Communication (HazCom) is the **#2 most cited OSHA violation** with 2,888 violations in FY2024. Common violations include:
- Lack of written hazard communication program
- No employee training on hazardous chemicals
- **Not having Safety Data Sheets (SDSs) readily accessible**
- No secondary container labeling

This project directly addresses SDS accessibility—a core HazCom requirement.

---

## Project Background

### Traditional Workflow (Before AI)

1. Walk facility, manually write down each chemical product
2. Research manufacturer websites to find SDS documents (15-30 min each)
3. Download, print, and organize into physical binder
4. Create index/table of contents
5. Train employees on binder location and usage

**Estimated time for 73 chemicals: 25-36 hours**

### AI-Assisted Workflow (This Project)

1. **Photo documentation:** Walked facility, photographed all chemical containers (~1-2 hours)
2. **Claude Cowork processing:** Uploaded photos; AI identified products, extracted manufacturer info, created structured spreadsheet (~30 min active time)
3. **SDS verification:** Reviewed AI-generated spreadsheet, verified SDS URLs (~2 hours)
4. **Claude Code development:** Built searchable web portal with categories, mobile support, and instant search (~4 hours collaboration)

**Actual time: ~8 hours**

### Time Savings

| Task | Traditional | AI-Assisted | Reduction |
|------|-------------|-------------|-----------|
| Inventory documentation | 3-4 hrs | 1-2 hrs | 50% |
| SDS research per chemical | 15-20 min × 73 | Auto-generated | 85% |
| System creation | 4-8 hrs | ~4 hrs | 50% |
| **Total** | **25-36 hrs** | **~8 hrs** | **~75%** |

---

## Cost Analysis

### SDS Management Software Market Research

Commercial SDS management solutions require ongoing subscriptions. Based on current market pricing:

| Vendor | Pricing Model | Annual Cost | Source |
|--------|---------------|-------------|--------|
| [SDS Manager](https://sdsmanager.com/us/pricing/) | Volume-based | $468/yr (100 SDS) to $2,064/yr (1,000 SDS) | Public pricing page |
| [mSDS Source](https://www.msdssource.com/pricing) | Flat rate | $1,299/yr (Red Level) | Public pricing page |
| [VelocityEHS](https://www.capterra.com/p/88891/EHS-Management-Software/) | Quote-based | Not publicly disclosed (enterprise pricing) | Capterra |
| [Chemwatch](https://slashdot.org/software/comparison/Chemwatch-vs-VelocityEHS/) | Quote-based | Not publicly disclosed | Vendor comparison |

**Note:** Enterprise solutions like VelocityEHS and Chemwatch do not publish pricing. Based on industry reports and user reviews, enterprise EHS platforms typically range from $2,000-$10,000+/year depending on modules and company size.

### Our Solution Cost

| Item | Cost |
|------|------|
| Vercel hosting | $0 (free tier) |
| Domain | $0 (using Vercel subdomain) |
| Maintenance | Internal (minimal) |
| **Annual Total** | **$0** |

### Conservative 5-Year Comparison

| Solution | Year 1 | Years 2-5 | 5-Year Total |
|----------|--------|-----------|--------------|
| Budget SDS software (~$500/yr) | $500 | $2,000 | $2,500 |
| Mid-tier SDS software (~$1,300/yr) | $1,300 | $5,200 | $6,500 |
| Enterprise platform (~$3,000/yr) | $3,000 | $12,000 | $15,000 |
| **Our AI-built solution** | **$0** | **$0** | **$0** |

---

## Legal Compliance

### Federal OSHA Requirements (29 CFR 1910.1200)

The Hazard Communication Standard requires employers to:

> "Ensure that safety data sheets are readily accessible during each work shift to employees when they are in their work area."

Source: [OSHA 1910.1200](https://www.osha.gov/laws-regs/regulations/standardnumber/1910/1910.1200)

**How our portal complies:**
- ✅ SDSs accessible from any device (phone, tablet, computer)
- ✅ Available 24/7 during all work shifts
- ✅ Instant search by chemical name, manufacturer, or CAS number
- ✅ No login required—immediate access

### California Cal/OSHA Requirements (Title 8, Section 5194)

Cal/OSHA's Hazard Communication Standard requires:

> "Employers are required to provide information to their employees about the hazardous substances to which they may be exposed, by means of a hazard communication program, labels and other forms of warning, safety data sheets and employee training."

Source: [Cal/OSHA Section 5194](https://www.dir.ca.gov/title8/5194.html)

**How our portal complies:**
- ✅ Centralized SDS repository for all workplace chemicals
- ✅ Organized by category (Solvents, Adhesives, Lubricants, etc.)
- ✅ Prop 65 chemicals flagged in dedicated section
- ✅ Emergency contact numbers (911, Poison Control) always visible

### Digital SDS Compliance Note

OSHA allows electronic/digital SDS access, but requires:

> "If you choose to have a digital copy of your SDS, you must have a backup available in case of a power outage or equipment failure. OSHA also requires you to train your workforce to access the SDSs if you store them in digital format."

**Our compliance approach:**
- Digital portal serves as primary quick-access tool
- Physical binder maintained on-site as backup
- Employees trained on both access methods during onboarding

---

## Risk Mitigation: OSHA's #2 Most Cited Violation

### Current Violation Statistics

According to [OSHA's Top 10 Most Cited Standards](https://www.osha.gov/top10citedstandards) for FY2024:

| Rank | Standard | Violations |
|------|----------|------------|
| 1 | Fall Protection (1926.501) | 6,307 |
| **2** | **Hazard Communication (1910.1200)** | **2,888** |
| 3 | Ladders (1926.1053) | 2,573 |
| 4 | Respiratory Protection (1910.134) | 2,470 |
| 5 | Lockout/Tagout (1910.147) | 2,443 |

Hazard Communication has ranked in the **top 3 for three consecutive years** (2022-2024).

### Penalty Exposure

As of January 15, 2025, per [OSHA Penalties](https://www.osha.gov/penalties):

| Violation Type | Maximum Penalty |
|----------------|-----------------|
| Serious / Other-than-serious | $16,550 per violation |
| Willful or repeated | $165,514 per violation |
| Failure to abate | $16,550 per day |

**Real-world context:** According to industry reports, average HazCom penalties in inspected workplaces range from [$7,000-$10,000 per violation](https://www.printing.org/content/2025/04/15/the-top-10-osha-violations-in-printing-for-2024---and-what-they-mean-for-your-shop).

### How This Project Reduces Risk

| Common HazCom Citation | Our Mitigation |
|------------------------|----------------|
| SDSs not readily accessible | Instant mobile/web access from anywhere |
| Employees don't know where SDSs are | Single memorable URL: ehsbot.vercel.app |
| SDSs outdated or missing | Easy update workflow (see MAINTENANCE.md) |
| No written HazCom program | Portal documents chemical inventory |

---

## Employee Onboarding Integration

### OSHA Training Requirements

Per [OSHA's Hazard Communication training requirements](https://www.osha.gov/sites/default/files/publications/OSHA3642.pdf):

> "Employees must receive training on hazardous chemicals at the time of their initial assignment, and whenever a new chemical hazard is introduced into their work area."

Training must cover:
- Location and availability of SDSs
- How to access and use SDS information
- Understanding SDS format (16-section structure)

### First-Day Safety Onboarding Checklist

Use this checklist for new hire orientation:

```
□ Show employee the SDS Portal: ehsbot.vercel.app
□ Demonstrate search function (by name, manufacturer, or CAS#)
□ Explain category organization (Solvents, Adhesives, etc.)
□ Point out emergency numbers in header (911, Poison Control)
□ Show physical binder location (backup)
□ Have employee bookmark portal on their phone
□ Document training completion
```

### Why Digital Access Matters for Onboarding

| Traditional Binder | Digital Portal |
|--------------------|----------------|
| "The binder is in the break room" | "Go to ehsbot.vercel.app on your phone" |
| Requires walking to fixed location | Accessible from workstation |
| One person can use at a time | Unlimited simultaneous access |
| Flipping through alphabetical tabs | Instant search results |
| May not be updated | Last updated date visible |

---

## People Team Utilization Guide

### How HR/People Ops Can Use This Tool

#### 1. New Hire Orientation Module

Add the SDS Portal to your standard onboarding checklist:

**Day 1 Safety Orientation:**
- [ ] Complete HazCom training video (if applicable)
- [ ] Review SDS Portal access (ehsbot.vercel.app)
- [ ] Demonstrate search and navigation
- [ ] Employee signs acknowledgment of SDS access training

#### 2. Training Documentation

Create a simple acknowledgment form:

```
SAFETY DATA SHEET ACCESS ACKNOWLEDGMENT

I, _________________, acknowledge that on _______ (date) I received training on:

☑ The location of our digital SDS Portal (ehsbot.vercel.app)
☑ How to search for chemical safety information
☑ The location of the physical SDS binder backup
☑ Emergency contact numbers (911, Poison Control: 1-800-222-1222)

I understand that Safety Data Sheets must be reviewed before working with
any hazardous chemical and are available 24/7 via the portal.

Signature: _________________ Date: _________
```

#### 3. Annual Refresher Training

During annual safety refreshers:
- Verify employees can still access the portal
- Review any new chemicals added since last training
- Confirm physical binder backup location

#### 4. Incident Response Reference

In case of chemical exposure or spill:
1. Employee can immediately pull up SDS on phone
2. First responders/medical personnel have instant access
3. No delay searching for physical binder during emergency

#### 5. Compliance Audits

When preparing for OSHA inspections or internal audits:
- Portal shows "Last Updated" date (demonstrates active maintenance)
- Chemical count displayed (73 chemicals indexed)
- Categories show organized hazard communication program
- Easy to demonstrate employee access during walkthrough

---

## AI Use Case Documentation

### Tools Used

| Tool | Purpose | Outcome |
|------|---------|---------|
| **Claude Cowork** | Photo analysis, data extraction, spreadsheet generation | Converted 73+ product photos into structured inventory |
| **Claude Code** | Web development, code generation, deployment | Built production-ready SDS portal |
| **Vercel** | Hosting | Free, instant global deployment |
| **GitHub** | Version control | Change tracking, easy rollback |

### AI Capabilities Demonstrated

1. **Computer Vision → Structured Data**
   - Input: Photos of chemical containers
   - Output: Spreadsheet with product names, manufacturers, hazard info

2. **Natural Language → Functional Code**
   - Input: "Build a searchable SDS portal with categories and mobile support"
   - Output: Complete single-page application (~1,500 lines)

3. **Iterative Refinement**
   - Added features through conversation (alphabetical index, dark theme, emergency contacts)
   - Removed features when scope creep threatened simplicity

4. **Documentation Generation**
   - Maintenance cheat sheet created automatically
   - This use case document generated from project context

### Replicability

This workflow can be applied to other EHS documentation needs:
- Equipment inspection checklists
- PPE inventory management
- Training record tracking
- Incident reporting systems
- Regulatory permit tracking

---

## Business Case for Enterprise AI Licensing

### ROI Summary

| Metric | Value |
|--------|-------|
| Development time saved | ~20-28 hours |
| Labor cost avoided (@ $50/hr) | $1,000 - $1,400 |
| SaaS subscription avoided (Year 1) | $500 - $3,000 |
| 5-year SaaS savings | $2,500 - $15,000 |
| Risk mitigation value | Avoids $7,000-$16,550 per HazCom citation |

### Qualitative Benefits

- **Speed:** Hours instead of weeks to deploy compliance tools
- **Ownership:** Full control of code and data (no vendor lock-in)
- **Customization:** Tailored to our specific chemical inventory
- **Simplicity:** Single-file architecture, no complex infrastructure
- **Maintainability:** Non-technical staff can update with simple workflow

### Justification Statement

> "Using Claude Cowork for photo-to-data extraction and Claude Code for web development, I completed a full chemical inventory and deployed a compliant digital SDS portal in approximately 8 hours—a 75% reduction from traditional methods. The solution directly addresses OSHA's #2 most cited violation (Hazard Communication), costs nothing to operate, and eliminates the need for a $500-$3,000+/year SDS management subscription. This project demonstrates measurable productivity gains and compliance value that would scale across other EHS documentation workflows with enterprise AI access."

---

## Appendix: Project Files

| File | Purpose |
|------|---------|
| `index.html` | Complete SDS Portal application |
| `MAINTENANCE.md` | Update workflow cheat sheet |
| `AI_EHS_USE_CASE_PROJECT.md` | This document |

**Repository:** https://github.com/MS-707/EHSBOT
**Live Site:** https://ehsbot.vercel.app/

---

## Sources

- [OSHA Top 10 Most Cited Standards](https://www.osha.gov/top10citedstandards)
- [OSHA Hazard Communication Standard 1910.1200](https://www.osha.gov/laws-regs/regulations/standardnumber/1910/1910.1200)
- [OSHA Penalties](https://www.osha.gov/penalties)
- [Cal/OSHA Title 8 Section 5194](https://www.dir.ca.gov/title8/5194.html)
- [Cal/OSHA Hazard Communication Regulation (PDF)](https://www.dir.ca.gov/dosh/dosh_publications/hazcom.pdf)
- [SDS Manager Pricing](https://sdsmanager.com/us/pricing/)
- [mSDS Source Pricing](https://www.msdssource.com/pricing)
- [VelocityEHS - Capterra](https://www.capterra.com/p/88891/EHS-Management-Software/)
- [OSHA HazCom Training Requirements](https://www.osha.gov/sites/default/files/publications/OSHA3642.pdf)

---

*Document generated with Claude Code | January 2026*
