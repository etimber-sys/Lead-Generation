# Clay.com — Platform Capabilities for Lead Generation
**Sources:** Clay.com, Clay University, Clay Integrations Page
**Research Date:** April 2026

---

## Important Clarification

> **Note:** The PRD references "Clay.com" as the website platform, but the search results indicate that Clay.com (clay.com) is actually a **B2B data enrichment and outreach automation platform** — not a website builder. The project team should clarify whether they are using:
> - **Clay.com** (data/outreach tool) — for enriching and automating lead outreach
> - **Another "Clay" platform** — e.g., a website builder that uses the Clay name

The findings below describe Clay.com (the data/outreach platform).

---

## What Clay.com Does

Clay is a go-to-market data enrichment and workflow automation platform:

> "Access 150+ premium data sources and AI research agents in one platform, then automate growth workflows to turn insights into revenue."

**Core capabilities:**
- 50+ built-in data providers (titles, work emails, departments, headcount growth)
- 150+ premium data sources for lead enrichment
- AI research agents for automated prospecting
- Cold outreach automation (find leads → enrich → personalize → send)
- HTTP API for custom integrations without code

---

## Forms & Lead Capture

Clay is **not a form builder**. It integrates with third-party form tools rather than providing native form creation.

**Confirmed integrations:**
- **Typeform** — Native integration; forms can be embedded in websites, newsletters, or shared on social media; Clay processes inbound form submissions automatically

> "Typeform is a popular tool for capturing inbound leads. Forms can be easily embedded in websites, newsletters, or surfaced on social media. Clay has a native [Typeform integration]."

---

## Integrations

| Integration | Purpose |
|---|---|
| Typeform | Inbound lead capture forms |
| Gong Engage | Push contacts to sales engagement flows |
| HTTP API | Build custom integrations without code |
| 50+ data providers | Lead enrichment (email, title, company data) |

> "Clay + Gong Engage integration allows users to seamlessly push contacts from their Clay tables directly into Gong Engage Flows, enhancing workflow efficiency."

---

## Gated Content / Conditional Logic

- **No native gated content** support in Clay.com
- **No native conditional logic forms** — Clay relies on Typeform or similar tools for this
- Conditional logic must be built within the connected form tool (e.g., Typeform)

---

## GA4 / Analytics Integration

- **Not confirmed** in available search results
- Clay does not appear to have native GA4 integration
- Analytics tracking would need to be handled by the website platform the forms are embedded in

---

## Lead Generation Workflow (How Clay Is Typically Used)

1. **Find leads** — Search Clay's data providers for target companies/contacts
2. **Enrich leads** — Pull emails, titles, company info, growth signals
3. **Personalize outreach** — AI writes personalized messages per lead
4. **Send emails** — Automated outreach sequences

> "With our AI lead generation workflows—including finding leads, enriching them, and sending personalized emails—you can skyrocket your cold outreach success."

---

## Recommended Third-Party Stack (if using Clay.com)

| Need | Recommended Tool |
|---|---|
| Website/landing pages | Webflow, Framer, or existing platform |
| Multi-step forms | Typeform (native Clay integration) |
| Conditional logic forms | Typeform or Fillout |
| Gated content delivery | Typeform + email automation |
| GA4 tracking | Embed GA4 on website separately |
| CRM | HubSpot, Salesforce (via Clay enrichment) |
| Email nurture | Instantly, Smartlead, or HubSpot |

---

## Action Item for Project Team

Clarify the exact platform being used for the website. If the site is not Clay.com (data tool), identify the actual website builder to assess:
- Native form capabilities
- Gated content support
- GA4 embed options
- Integration with Typeform or HubSpot forms
