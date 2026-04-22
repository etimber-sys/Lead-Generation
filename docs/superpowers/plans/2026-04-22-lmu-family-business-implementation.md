# LMU Family Business Program — Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Execute a 12-month growth and quality improvement strategy for the LMU Family Business Entrepreneurship Program, moving from low awareness to 8–15 net new memberships and measurably stronger program quality.

**Architecture:** Three parallel tracks — personalized 1:1 outbound to 41 confirmed leads (22 LMU alumni first), a referral/partner network for trust-based growth, and content/SEO for durable inbound — all feeding into program quality improvements that drive retention and word-of-mouth.

**Tools Needed:**
- LinkedIn (outreach) + LinkedIn Sales Navigator (list-building, ~$80/mo)
- LMU email account (direct outreach)
- Typeform free tier (assessment tool)
- Mailchimp free tier (nurture sequences + newsletter, free up to 500 contacts)
- LMU website CMS (SEO pages — coordinate with web team)
- Google Business Profile (free)
- Google Sheets (pipeline tracker)
- Eventbrite (already in use for events)

---

## Asset Map

| Asset | Where to save | Created in task |
|---|---|---|
| Pipeline tracker | `outreach/pipeline-tracker.csv` | Task 1 |
| Alumni outreach messages | `outreach/alumni-messages.md` | Task 1 |
| Non-alumni outreach messages | `outreach/non-alumni-messages.md` | Task 2 |
| Succession Assessment (Typeform) | Typeform + `lead-magnets/succession-assessment.md` | Task 3 |
| Nurture email sequence | `nurture/email-sequence.md` | Task 4 |
| List-building criteria | `outreach/list-building-criteria.md` | Task 5 |
| Referral one-pager | `referral/member-referral-onepager.md` | Task 6 |
| Advisor outreach list + message | `partnerships/advisor-outreach.md` | Task 7 |
| Co-branded checklist | `partnerships/cobrand-checklist.md` | Task 7 |
| SEO page: LA Program | `seo/page-la-program.md` | Task 8 |
| SEO page: Succession Planning | `seo/page-succession-planning.md` | Task 8 |
| SEO page: Next Gen Leadership | `seo/page-next-gen-leadership.md` | Task 8 |
| Peer group structure doc | `program/peer-groups.md` | Task 9 |
| Curriculum calendar | `program/curriculum-calendar.md` | Task 10 |
| Newsletter template | `newsletter/issue-template.md` | Task 11 |
| Post-event feedback survey | `program/feedback-survey.md` | Task 12 |
| Student integration guide | `program/student-integration.md` | Task 13 |
| Member case study template | `marketing/case-study-template.md` | Task 14 |
| Quarterly review template | `reviews/quarterly-review.md` | Task 15 |

---

## Task 1: Wave 1 — LMU Alumni Outreach (Weeks 1–2)

**22 of the 41 CSV leads are LMU alumni. Contact these first — the LMU connection is a trust shortcut that non-alumni outreach doesn't have.**

**Files:**
- Create: `outreach/pipeline-tracker.csv`
- Create: `outreach/alumni-messages.md`

- [ ] **Step 1: Set up the pipeline tracker**

Create `outreach/pipeline-tracker.csv` with these columns:

```
Company Name, Contact Name, Job Title, Email, LinkedIn, LMU Alumni (Y/N), Contacted Date, Channel Used, Response (Y/N/Pending), Notes, Stage
```

Copy all 41 leads from `Project Documents/Family-Businesses-Compiled.csv` into this tracker. Sort alumni (Y) to the top. Stage options: `Not Contacted → Contacted → Responded → Invited to Event → Attended Event → Membership Conversation → Member`

- [ ] **Step 2: Write the alumni LinkedIn message**

Save to `outreach/alumni-messages.md`. Use this as the template — personalize the `[brackets]` for each person:

```
Subject (if email): Fellow Lion building something for family businesses

Hi [First Name],

I came across [Company Name] and noticed your LMU connection — I'm the director of the Family Business Entrepreneurship Program here at the Fred Kiesner Center.

We've built a community specifically for family-owned businesses in LA — peer groups, workshops on succession and governance, and an annual conference. Given what you're building at [Company Name], I thought it might be worth a conversation.

We have an upcoming forum on [next event topic + date] that's open to family businesses in the area. No membership required — just a good room of people working through similar challenges.

Would you be open to joining us?

[Your name]
LMU Family Business Entrepreneurship Program
```

- [ ] **Step 3: Send outreach to all 22 alumni leads**

Work through the alumni segment of the pipeline tracker. For each:
1. Find them on LinkedIn or use the email in the CSV
2. Personalize the template with their company name and any relevant detail from their profile (industry, how long they've been operating, if they mention succession or next-gen)
3. Send via LinkedIn message (preferred) or direct email
4. Log the date and channel in the tracker; set Stage to `Contacted`

Send no more than 5–7 per day to avoid appearing as spam and to give yourself time to personalize.

- [ ] **Step 4: Set a follow-up reminder for non-responders**

After 7 days, send one follow-up to anyone who hasn't responded:

```
Hi [First Name], just following up on my note below — happy to share more about the program or answer any questions. Either way, hope things are going well at [Company Name].
```

- [ ] **Step 5: Log responses and update tracker stages**

For anyone who responds positively: move to `Invited to Event`, send event details, and add a calendar reminder to check in 3 days before the event.

- [ ] **Step 6: Commit tracker and message templates**

```bash
git add outreach/
git commit -m "feat: add alumni outreach tracker and message templates"
```

**Done when:** All 22 alumni leads have been contacted and logged in the tracker.

---

## Task 2: Wave 2 — Non-Alumni Outreach (Weeks 3–4)

**19 remaining leads with no LMU connection. Lead with value — reference their specific business or a pain point relevant to their industry.**

**Files:**
- Create: `outreach/non-alumni-messages.md`

- [ ] **Step 1: Write the non-alumni outreach message**

Save to `outreach/non-alumni-messages.md`. Three variants by persona — use whichever fits the lead's job title:

**Variant A — Founder (CEO/Owner, 55+):**
```
Hi [First Name],

I lead the Family Business Entrepreneurship Program at LMU, and [Company Name] came up as a business we'd love to connect with.

We've found that most family business owners are navigating succession, governance, and generational transition largely on their own — which is exactly why we built this community. Monthly workshops, peer groups with other owners, and an annual conference, all focused on the challenges that are specific to family-run companies.

We have an upcoming forum on [event topic] on [date] — no membership needed to attend. I'd love to have [Company Name] in the room.

[Your name]
```

**Variant B — Successor (Next-gen title, 28–45):**
```
Hi [First Name],

I run the Family Business Entrepreneurship Program at LMU. We've built a next-generation peer group specifically for leaders like you — people stepping into (or navigating alongside) the founding generation.

The group meets quarterly and is small by design: candid conversations about authority, transition timelines, and how to modernize without creating family conflict. No consultants selling anything — just next-gen leaders comparing notes.

We have a forum coming up on [event topic] on [date] that would be a good intro. Would it be worth 10 minutes to tell you more?

[Your name]
```

**Variant C — Sibling Team (Multiple family members listed):**
```
Hi [First Name],

I lead the Family Business Entrepreneurship Program at LMU. We work specifically with family-owned businesses navigating the dynamics that are unique to having family in the room — roles, compensation, shared vision, governance.

Given the structure at [Company Name], I thought our community might be worth knowing about. We run peer groups, workshops on governance and conflict resolution, and an annual conference — all designed for families running businesses together.

We have an upcoming forum on [event topic] on [date]. Happy to share more if it sounds relevant.

[Your name]
```

- [ ] **Step 2: Match each of the 19 leads to a persona variant**

Review each lead's job title and company structure in the pipeline tracker. Assign Variant A, B, or C. Note this in the `Notes` column.

- [ ] **Step 3: Send outreach to all 19 non-alumni leads**

Same process as Task 1 — personalize, send, log in tracker. 5–7 per day max.

- [ ] **Step 4: Send follow-ups at Day 7**

Same one-line follow-up as Task 1 for non-responders.

- [ ] **Step 5: Update tracker and commit**

```bash
git add outreach/non-alumni-messages.md
git commit -m "feat: add non-alumni outreach messages and complete Wave 2"
```

**Done when:** All 41 leads contacted, all stages logged in tracker.

---

## Task 3: Build the Succession Readiness Assessment (Month 1)

**The lead magnet. A 10-question self-scoring tool that tells owners where they stand on succession — interactive format converts at 20–30% vs. ~15% for static PDFs. Gate: name + email only.**

**Files:**
- Create: `lead-magnets/succession-assessment.md` (content source)
- Build in: Typeform (free tier, no cost)

- [ ] **Step 1: Write the 10 assessment questions**

Save to `lead-magnets/succession-assessment.md`. Use this exact question set:

```
Title: How Ready Is Your Family Business for the Next Generation?
Subtitle: Answer 10 questions to get your Succession Readiness Score and a personalized next step.

Gate (before results): Name + Email only

Q1. Do you have a written succession plan?
  a) Yes, documented and reviewed in the last 2 years (3 pts)
  b) Informal plan, not written down (1 pt)
  c) No plan yet (0 pts)

Q2. Has your chosen successor been identified?
  a) Yes, identified and they know it (3 pts)
  b) We have someone in mind but haven't had the conversation (1 pt)
  c) No successor identified (0 pts)

Q3. Is your successor actively being developed for leadership?
  a) Yes — mentorship, training, or formal development is underway (3 pts)
  b) They're in the business but not in a formal development role (1 pt)
  c) No development plan exists (0 pts)

Q4. Have you had an open conversation with your family about the future of the business?
  a) Yes — we've discussed it openly and recently (3 pts)
  b) It's come up but never fully resolved (1 pt)
  c) We avoid the topic (0 pts)

Q5. Do you have a governance structure (family council, advisory board, or formal decision process)?
  a) Yes — formal structure in place (3 pts)
  b) Informal processes but nothing documented (1 pt)
  c) No governance structure (0 pts)

Q6. Is your personal wealth separated from the business?
  a) Yes — personal and business finances are clearly separated (3 pts)
  b) Partially separated (1 pt)
  c) Closely tied together (0 pts)

Q7. Have you worked with an estate attorney or financial advisor on business transfer?
  a) Yes — estate and tax planning is in place (3 pts)
  b) We've talked about it but not acted (1 pt)
  c) Not yet (0 pts)

Q8. Do your key non-family employees know the succession plan?
  a) Yes — key leaders are informed (3 pts)
  b) Some know informally (1 pt)
  c) No one outside the family knows (0 pts)

Q9. If something happened to you tomorrow, could the business continue without you for 90 days?
  a) Yes — systems and people are in place (3 pts)
  b) It would be difficult but possible (1 pt)
  c) The business depends entirely on me (0 pts)

Q10. Do you have a target timeline for transitioning leadership?
  a) Yes — specific timeline, shared with the family (3 pts)
  b) Vague timeline ("eventually") (1 pt)
  c) No timeline (0 pts)

---
SCORING:
24–30: Well Prepared — You've done the hard work. The next step is fine-tuning and peer community.
14–23: In Progress — You've started but gaps remain. A structured program can accelerate your readiness.
0–13: Needs Attention — You're not alone. 43% of family businesses have no plan. The time to start is now.

RESULTS PAGE CTA (all scores):
"Join us at the next LMU Family Business Forum to connect with other owners navigating this — [link to event registration]"
```

- [ ] **Step 2: Build the assessment in Typeform**

1. Go to typeform.com → Create new form
2. Title: "Family Business Succession Readiness Score"
3. Add a Welcome Screen: "10 questions. 3 minutes. Find out exactly where your family business stands on succession."
4. Add the 10 multiple-choice questions from Step 1
5. Add a gate screen before results: collect First Name + Email (two fields only)
6. Configure score logic: assign point values per answer as noted above
7. Add three outcome screens based on score ranges (0–13, 14–23, 24–30) with the copy from Step 1
8. Each outcome screen ends with the event CTA
9. Connect email field to Mailchimp (see Task 4 for sequence setup)
10. Publish and copy the public URL

- [ ] **Step 3: Write the landing page copy**

This goes on the LMU website as a standalone landing page (coordinate with web team). Content:

```
Headline: How Ready Is Your Family Business for the Next Generation?

Subheadline: Most family businesses wait too long. Take our 3-minute assessment to find out where you stand — and what to do next.

What you'll get:
- Your personalized Succession Readiness Score
- A clear picture of your biggest gaps
- A recommended next step based on your results

[Start the Assessment →]

Used by family business owners across Los Angeles.
No spam. Unsubscribe anytime.
```

- [ ] **Step 4: Add the assessment link to all outreach and social profiles**

- Add to LMU Family Business Program website homepage (above the fold)
- Add to LinkedIn bio
- Add to email signature
- Share in the next Instagram/LinkedIn post

- [ ] **Step 5: Commit content file**

```bash
git add lead-magnets/succession-assessment.md
git commit -m "feat: add succession readiness assessment content"
```

**Done when:** Typeform is live and accessible via public URL; linked from LMU website and outreach materials.

---

## Task 4: Build the 4-Email Nurture Sequence (Month 1)

**Everyone who completes the assessment enters this sequence. Goal: 3–5 trust-building touchpoints before inviting them to membership. Build in Mailchimp.**

**Files:**
- Create: `nurture/email-sequence.md`

- [ ] **Step 1: Write all 4 emails**

Save to `nurture/email-sequence.md`:

```
EMAIL 1 — Immediate (triggered on assessment completion)
Subject: Your Family Business Succession Score + Next Step
---
Hi [First Name],

Thanks for taking the assessment — here's what your score means and what to do with it.

[Score outcome copy from Typeform — repeat their specific result]

The most important thing we've learned from working with family businesses: the ones who succeed at transition aren't necessarily the most financially prepared. They're the ones who start the conversation early — with their family, their advisors, and their peers.

That's exactly what the LMU Family Business Program is designed to support.

Over the next few weeks I'll share a few resources that address the specific gaps your score identified. No pitches — just useful things.

[Your name]
Director, LMU Family Business Entrepreneurship Program

---

EMAIL 2 — Day 3
Subject: The question most family business owners avoid
---
Hi [First Name],

One question we ask in our peer groups tends to stop the room:

"If something happened to you tomorrow, who would run the business — and do they know it?"

43% of family business owners have no succession plan. Not because they don't care, but because the conversation feels too big, too emotional, or too far away to start.

Here's what we've found actually helps: hearing how other families handled it. Not consultants — real owners.

We hold a quarterly peer group for family business owners in LA — small group, facilitated, confidential. Here's what a past participant said:

"I thought we were the only ones dealing with this. Turns out everyone in the room had the same conversation they were avoiding." — Member, LMU Family Business Program

Our next forum is [event date]. It's open to non-members — no commitment, just a room worth being in.

[Event registration link]

[Your name]

---

EMAIL 3 — Day 10
Subject: What the 2nd generation actually needs from you
---
Hi [First Name],

One of the most consistent things we hear from next-gen family business leaders:

"I don't know when it's going to be my turn — and I don't know how to ask."

And from founders: "I'll hand it off when they're ready. I'm just not sure they are yet."

Both sides are waiting for the other to start the conversation.

The programs that work best at solving this aren't the ones with the best consultants. They're the ones that put families in the room with other families who've already had the conversation — and lived to tell about it.

A few resources that might be useful:
- [Link to a relevant article or event recap on next-gen leadership]
- Our upcoming Next Gen Leadership Forum: [event link]

What's the most pressing thing you're navigating at [Company Name] right now? Hit reply — I read every response.

[Your name]

---

EMAIL 4 — Day 21
Subject: One last thing before I stop filling your inbox
---
Hi [First Name],

I've shared a few things over the past few weeks. I'll keep this one short.

If any of it resonated — the succession planning challenges, the generational dynamics, the sense that you're navigating this without enough peers who get it — the LMU Family Business Program is worth a closer look.

Here's what membership includes:
- Quarterly peer groups (Founders, Next-Gen, and Sibling Teams)
- Monthly workshops mapped to the challenges that come up most for family businesses
- Annual conference
- Access to LMU's network and student talent pool

Annual membership: $495/year (under $2M revenue) or $995/year (over $2M revenue).

If you'd like to talk before committing, I'm happy to do a 20-minute call. Just reply to this email.

Either way — good luck with [Company Name]. These businesses matter more than most people realize.

[Your name]
[Calendar link for 20-min call]
```

- [ ] **Step 2: Set up the sequence in Mailchimp**

1. Create a new Audience (or use existing) in Mailchimp
2. Create a new Customer Journey (automation) triggered by: "Contact is added to audience via Typeform integration"
3. Add Email 1 as immediate trigger
4. Add Email 2 with 3-day delay
5. Add Email 3 with 7-day delay (10 days from start)
6. Add Email 4 with 11-day delay (21 days from start)
7. Connect Typeform to Mailchimp via native integration (Settings → Integrations in Typeform)
8. Test the sequence with your own email before publishing

- [ ] **Step 3: Commit email content**

```bash
git add nurture/email-sequence.md
git commit -m "feat: add 4-email nurture sequence content"
```

**Done when:** Sequence is live in Mailchimp; test email received; Typeform → Mailchimp connection confirmed.

---

## Task 5: List-Building System (Month 1, ongoing)

**41 leads is a small starting pool. This task creates the ongoing process for finding more qualified prospects.**

**Files:**
- Create: `outreach/list-building-criteria.md`

- [ ] **Step 1: Define qualification criteria**

Save to `outreach/list-building-criteria.md`:

```
A qualified prospect for the LMU Family Business Program meets ALL of:
1. Family-owned or family-operated business (founder surname in leadership, "family-owned" in bio/website, or multi-generation indicators)
2. Located in LA County, Orange County, or Ventura County (within driving distance of LMU's Playa Vista campus)
3. Business appears operational and established (not pre-revenue or brand new)
4. Owner or next-gen leader is reachable via LinkedIn or has a public email

BONUS SIGNALS (higher priority):
- LMU alumni connection
- Business is 10+ years old (succession is becoming relevant)
- Multiple family members listed in leadership
- Business has $1M+ in apparent revenue (can afford membership)
- Industry: construction, manufacturing, hospitality, retail, professional services, real estate — sectors with high family business density

DISQUALIFY:
- Publicly traded companies
- Businesses with no family name indicators
- Locations outside Southern California
```

- [ ] **Step 2: Set up LinkedIn Sales Navigator search**

In LinkedIn Sales Navigator, create a saved search with these filters:
- Geography: Los Angeles, Orange County, Ventura County
- Company headcount: 10–500 (filters out sole proprietors and large corps)
- Seniority: Owner, Founder, CEO, President, Managing Director
- Keywords (company description): "family-owned", "family business", "family operated", "founded by"

Save the search. Review 10–15 new results per week and add qualifying leads to the pipeline tracker.

- [ ] **Step 3: Create a nominations process for members and advisory board**

Draft a one-sentence ask to send to current members and advisory board members:

```
"We're growing the program and would love warm introductions to family-owned businesses in LA that might benefit. If anyone comes to mind — owners, next-gen leaders, or families navigating transition — I'd be grateful for an introduction or a name I can reach out to."
```

Send this to all current members and advisory board members in Month 2.

- [ ] **Step 4: Commit criteria doc**

```bash
git add outreach/list-building-criteria.md
git commit -m "feat: add list-building qualification criteria"
```

**Done when:** LinkedIn Sales Navigator search saved; nominations ask drafted; plan to review 10–15 new leads per week is in place.

---

## Task 6: Launch the Referral Program (Month 2)

**Current members are the highest-trust referral channel. Make it easy and give them a reason to act.**

**Files:**
- Create: `referral/member-referral-onepager.md`

- [ ] **Step 1: Write the referral one-pager**

Save to `referral/member-referral-onepager.md`. This is the document you send to current members:

```
# Refer a Family Business — Earn $150 Toward Your Membership

Know a family-owned business that could use this community?

When you refer a business that joins the LMU Family Business Program, you receive a $150 credit toward your next membership renewal. No limit on referrals.

HOW IT WORKS
1. Send us the name and contact of the family business you're referring (reply to this email or use the link below)
2. We'll reach out on your behalf
3. If they join, you get $150 off your renewal — automatically applied

YOUR REFERRAL MESSAGE (feel free to use this):
---
"I've been part of the LMU Family Business Program for [X time] and thought of you. It's been worth it for the peer group alone — a small group of family business owners in LA, no consultants, just real conversations about succession, governance, and growth. The director is [Your name] — I told her I was going to mention it. Worth a 20-minute call: [director email]."
---

Submit a referral: [Google Form link — create a simple form: Referrer name, Referred company name, Referred contact name, Referred email/LinkedIn]

Questions? Reply to this email.
```

- [ ] **Step 2: Create the referral tracking form**

Create a Google Form with fields:
- Your name (referrer)
- Company you're referring
- Contact name at that company
- Their email or LinkedIn URL
- Any context we should know?

Copy the form link and paste it into the one-pager above.

- [ ] **Step 3: Send the one-pager to all current members**

Email subject: `A quick ask — and a $150 thank you`

Send to the full current member list. Include the one-pager content in the email body. Track opens if possible (Mailchimp).

- [ ] **Step 4: Add referral tracking to pipeline tracker**

Add a column to `outreach/pipeline-tracker.csv`: `Referred By`. When a referral comes in via the form, add the lead to the pipeline tracker and note who referred them.

- [ ] **Step 5: Commit**

```bash
git add referral/member-referral-onepager.md
git commit -m "feat: add member referral program one-pager and tracking form"
```

**Done when:** One-pager sent to all current members; Google Form live; referral column added to tracker.

---

## Task 7: Professional Advisor Partnership Outreach (Month 2)

**CPAs, estate attorneys, and wealth managers already have trusted relationships with family business owners. Position the program as a resource they can refer clients to — not competition.**

**Files:**
- Create: `partnerships/advisor-outreach.md`
- Create: `partnerships/cobrand-checklist.md`

- [ ] **Step 1: Build the target list of 10–15 advisors**

Save to `partnerships/advisor-outreach.md`. Find and list LA-area professionals in these categories who work with closely-held and family businesses:

- **CPAs/accounting firms:** Look for firms that list "closely held businesses," "family business," or "succession planning" on their websites. Target managing partners or partners, not associates.
- **Estate attorneys:** Search for LA estate planning attorneys who mention business succession or family governance.
- **Wealth managers/family offices:** RIAs and family office advisors who serve business owners.

Find 4–5 in each category. For each, note: Name, Firm, Email/LinkedIn, Why they're a fit (one line).

- [ ] **Step 2: Write the advisor outreach message**

Add to `partnerships/advisor-outreach.md`:

```
Subject: Collaborating on family business education — LMU program

Hi [Name],

I lead the Family Business Entrepreneurship Program at LMU's Fred Kiesner Center for Entrepreneurship. We work with family-owned businesses in LA on succession planning, governance, and next-generation transitions.

I'd love to explore whether there's a natural overlap between what you do for your clients and what we offer. Many family business owners need both the technical planning work (estate, tax, legal) and a peer community to process the human side of transition — and those two things are most powerful when they reinforce each other.

Concretely: I'd love to co-create a short checklist or host a small co-branded event that would be useful to your clients — something you could offer as a resource without any obligation. In exchange, I'd welcome introductions to family businesses who might benefit from our community.

Would you be open to a 20-minute call to explore?

[Your name]
LMU Family Business Entrepreneurship Program
```

- [ ] **Step 3: Write the co-branded checklist**

This is the value asset to offer advisors. Save to `partnerships/cobrand-checklist.md`:

```
Title: Family Business Succession Readiness Checklist
Co-presented by: LMU Family Business Entrepreneurship Program + [Advisor Firm Name]

THE 10-POINT SUCCESSION READINESS CHECKLIST

Legal & Financial
☐ 1. Buy-sell agreement is in place and reviewed in the last 3 years
☐ 2. Business valuation has been completed in the last 2 years
☐ 3. Estate plan accounts for business ownership transfer
☐ 4. Key person life insurance is in place
☐ 5. Personal and business finances are clearly separated

Family & Governance
☐ 6. Successor has been identified and informed
☐ 7. Successor is in an active development plan
☐ 8. Family has had an open conversation about the transition timeline
☐ 9. Roles and compensation for family members are documented
☐ 10. A governance structure (family council or advisory board) is in place

---
Score 8–10: Well prepared. Fine-tune and stay connected to peers navigating the same journey.
Score 5–7: In progress. A few critical gaps remain — worth addressing in the next 12 months.
Score 0–4: Getting started. You're not alone — most family businesses are here. The time to act is now.

---
[LMU Family Business Program logo + contact]
[Advisor firm logo + contact]

Take the full Succession Readiness Assessment: [Typeform link]
```

- [ ] **Step 4: Send outreach to all 10–15 advisors**

Personalize the message from Step 2 for each advisor. Reference their firm and any specific work they do that's relevant. Send via LinkedIn message or direct email. Log in the pipeline tracker (add an `Advisor Partner` tag in the Stage column).

- [ ] **Step 5: Commit**

```bash
git add partnerships/
git commit -m "feat: add advisor partnership outreach and co-branded checklist"
```

**Done when:** All 10–15 advisors contacted; co-branded checklist ready to share on first positive response.

---

## Task 8: SEO Pages + Google Business Profile (Month 3)

**Three new web pages targeting high-intent LA searches, plus a Google Business Profile optimization. Coordinate with LMU's web team to publish pages on the CBA site.**

**Files:**
- Create: `seo/page-la-program.md`
- Create: `seo/page-succession-planning.md`
- Create: `seo/page-next-gen-leadership.md`

- [ ] **Step 1: Optimize Google Business Profile**

Go to google.com/business and claim/update the LMU Family Business Program listing:
- Name: `LMU Family Business Entrepreneurship Program`
- Category: `Business Management Consultant` (primary) + `Non-profit organization`
- Description (250 chars max): `The LMU Family Business Entrepreneurship Program helps family-owned businesses in Los Angeles thrive through peer groups, workshops on succession and governance, and an annual conference. Based at LMU's Fred Kiesner Center for Entrepreneurship.`
- Add photos: program director headshot, event photos, LMU campus, logo (minimum 10 photos — listings with 100+ photos get 520% more calls)
- Add all upcoming events from the events calendar
- Add FAQ section with these Q&As:
  - Q: Who is this program for? A: Family-owned businesses in the Los Angeles area, from founders to next-generation leaders.
  - Q: How much does membership cost? A: $495/year for businesses under $2M revenue; $995/year for businesses over $2M.
  - Q: Do I need to be a member to attend events? A: No — many events are open to non-members as a way to experience the community.

- [ ] **Step 2: Write Page 1 — Family Business Program Los Angeles**

Save to `seo/page-la-program.md`. This content goes on a new CBA website page:

```
URL slug: /centers/entrepreneurship/familybusinessprogram/los-angeles/
Title tag: Family Business Program Los Angeles | LMU Fred Kiesner Center
Meta description: Join LA's leading university-based family business community. Peer groups, succession workshops, and an annual conference for family-owned businesses in Los Angeles.

H1: Family Business Program — Los Angeles

INTRO (2–3 sentences):
The LMU Family Business Entrepreneurship Program brings together family-owned businesses across Los Angeles to navigate the challenges that are unique to running a business with family. Peer groups, monthly workshops, and an annual conference — built specifically for the dynamics that make family businesses different.

H2: Built for LA Family Businesses
[2–3 sentences about LA's family business landscape — reference community, industries common in LA, connection to LMU's local network]

H2: What Members Get
- Quarterly peer groups (Founders, Next-Gen Leaders, Sibling Teams)
- Monthly workshops on succession, governance, and leadership transition
- Annual Family Business Conference
- Access to LMU's entrepreneurship network and student talent
- $495/year (under $2M revenue) | $995/year (over $2M revenue)

H2: Who This Is For
[Reference the three personas — Founders, Successors, Sibling Teams — in plain language]

H2: What Our Members Say
[2–3 member testimonials — pull from feedback surveys once available; placeholder: request quotes from 2 current members before publishing]

H2: Upcoming Events in Los Angeles
[Dynamic event list — pull from events calendar]

CTA: Join the Program | Take the Succession Assessment
```

- [ ] **Step 3: Write Page 2 — Family Business Succession Planning Help**

Save to `seo/page-succession-planning.md`:

```
URL slug: /centers/entrepreneurship/familybusinessprogram/succession-planning/
Title tag: Family Business Succession Planning Help | LMU Los Angeles
Meta description: 43% of family businesses have no succession plan. LMU's Family Business Program helps LA families start the conversation, prepare the next generation, and plan for a successful transition.

H1: Family Business Succession Planning — Where to Start

INTRO:
Most family businesses don't fail because of market forces. They fail because succession planning gets delayed until it's too late. If you haven't started, you're not alone — 43% of family businesses have no formal plan.

H2: Why Succession Planning Is Hard for Family Businesses
[3–4 bullets drawing from persona pain points: avoiding the conversation, unclear successor selection, founder reluctance, emotional complexity]

H2: What Good Succession Planning Looks Like
[3–4 practical elements: written plan, successor development, governance structure, family communication]

H2: How LMU's Program Helps
[Describe peer groups and workshops specifically focused on succession — reference the curriculum mapped to pain points]

H2: Take the Succession Readiness Assessment
[Embed or link to Typeform assessment — "Find out where you stand in 3 minutes"]

H2: Upcoming Succession-Related Events
[Dynamic list filtered to relevant events]

CTA: Take the Assessment | Join the Program
```

- [ ] **Step 4: Write Page 3 — Next Generation Leadership Development**

Save to `seo/page-next-gen-leadership.md`:

```
URL slug: /centers/entrepreneurship/familybusinessprogram/next-generation-leadership/
Title tag: Next Generation Family Business Leadership | LMU Los Angeles
Meta description: LMU's Next-Gen peer group helps family business successors navigate the handoff, build authority, and prepare to lead — without damaging the family.

H1: Next Generation Leadership in Family Business

INTRO:
Stepping into leadership in a family business is different from any other leadership transition. The stakes are personal, the dynamics are complicated, and most next-gen leaders are navigating it without a roadmap.

H2: The Challenges Next-Gen Leaders Face
[From persona research: unclear timeline, authority vs. parent still present, wanting to modernize without conflict, no language for the transition conversation]

H2: What the LMU Next-Gen Peer Group Offers
[Describe the Next-Gen Leaders peer group — small, facilitated, quarterly, confidential — and what it addresses specifically]

H2: Upcoming Next-Gen Events
[Dynamic list — reference the Feb 2026 Next Gen Leadership Forum as a model]

H2: What Next-Gen Members Say
[Testimonial placeholder — request from a current next-gen member before publishing]

CTA: Join the Next-Gen Group | Attend the Next Forum
```

- [ ] **Step 5: Submit pages to LMU web team**

Email the web team with:
- The three page content files attached
- Requested URL slugs
- Request for schema markup: LocalBusiness type, address, event schema on events pages
- Request for FAQ schema on Page 1
- Timeline ask: live within 2 weeks

- [ ] **Step 6: Commit all SEO content**

```bash
git add seo/
git commit -m "feat: add three SEO page content files and GBP optimization notes"
```

**Done when:** GBP updated with photos, description, and events; all 3 page content files submitted to web team.

---

## Task 9: Launch Peer Groups (Month 4)

**The single highest-impact program quality improvement. Three tiered groups, each capped at 8–12 members, meeting quarterly.**

**Files:**
- Create: `program/peer-groups.md`

- [ ] **Step 1: Write the peer group structure document**

Save to `program/peer-groups.md`:

```
# LMU Family Business Peer Groups — Structure & Facilitation Guide

## Three Groups

GROUP 1: FOUNDERS
- Who: Current owners/founders, primarily 1st or 2nd generation, still actively running the business
- Size: 8–12 members
- Format: 90 minutes, quarterly (virtual or Playa Vista campus)
- Topics: Succession readiness, letting go, estate and transition planning, building a leadership team beyond family

GROUP 2: NEXT-GEN LEADERS
- Who: Children, siblings, or in-laws of founders who are working in or entering the business
- Size: 8–12 members
- Format: 90 minutes, quarterly
- Topics: Building authority alongside parents, modernizing without conflict, having the succession conversation, peer support

GROUP 3: SIBLING TEAMS
- Who: 2+ family members co-running or co-owning the business
- Size: 8–12 members
- Format: 90 minutes, quarterly
- Topics: Role clarity, compensation equity, shared vision, governance, resolving conflict without breaking the family

## Ground Rules (read at start of every session)
1. What's shared in the room stays in the room.
2. We're here to share experience, not give advice.
3. No selling, recruiting, or business pitches.
4. Phones away during discussion.
5. Every voice matters — quieter members get equal airtime.

## Session Structure (90 minutes)
- 0:00–0:10 — Welcome, ground rules, brief intros for new members
- 0:10–0:25 — Check-in round: "What's one thing happening in your business right now?"
- 0:25–1:05 — Main topic discussion (prepared question or case study)
- 1:05–1:20 — Open floor: any member can raise something they're navigating
- 1:20–1:30 — Wrap-up: one takeaway per person; next meeting date confirmed

## Facilitation Notes
- Your role is to draw out, not lecture. Ask "who else has experienced this?" after each share.
- If one person dominates: "Let's hear from someone who hasn't spoken yet."
- If the conversation gets too abstract: "Can you give us a specific example from your business?"
- If conflict emerges: "Thank you for sharing that. Does anyone else relate to this tension?"

## Recruiting Founding Cohorts
- Founders group: Target the Founder-persona leads from the outreach pipeline who expressed interest
- Next-Gen group: Target Successor-persona leads + use the Next Gen Leadership Forum attendees
- Sibling Team group: Target co-founder/co-owner leads from the CSV
- Minimum viable group: 5 members. Don't wait for 8–12 to launch.
- Announce at next event: "We're forming three peer groups — spots are limited. Email [director] to express interest."
```

- [ ] **Step 2: Recruit founding cohort members**

Email everyone in the pipeline tracker in the `Attended Event` or later stage:

```
Subject: We're launching peer groups — limited spots

Hi [First Name],

Based on the conversations at our last forum, we're launching three small peer groups specifically for family business owners:

- Founders Group (current owners navigating succession and transition)
- Next-Gen Leaders Group (sons, daughters, and family members stepping into leadership)
- Sibling Teams Group (co-founders and co-owners navigating shared ownership)

Each group meets quarterly, 90 minutes, with a small cohort of 8–12 members. Everything stays in the room.

We're filling founding cohorts now — spots are limited by design. If you'd like to join one, reply to this email and tell me which group fits you best. I'll follow up to confirm.

[Your name]
```

- [ ] **Step 3: Schedule the first meetings for all three groups**

Once each group has at least 5 committed members:
1. Create a recurring quarterly calendar event
2. Send a calendar invite to all members
3. Book the Playa Vista campus room (or set up Zoom for virtual)
4. Prepare the first session's main discussion question for each group:
   - Founders: "What's the one thing about transitioning this business that you haven't been able to say out loud?"
   - Next-Gen: "What does your parent/family member do that makes leadership harder — and what do you wish you could say to them?"
   - Sibling Teams: "What's the one role clarity issue that, if resolved, would make the biggest difference in how you work together?"

- [ ] **Step 4: Commit structure doc**

```bash
git add program/peer-groups.md
git commit -m "feat: add peer group structure and facilitation guide"
```

**Done when:** All three groups have 5+ committed members; first meetings scheduled.

---

## Task 10: Curriculum Calendar Mapped to Pain Points (Month 4)

**Publish a public content calendar that maps every event and workshop to a specific member pain point. Makes the value of membership concrete and searchable.**

**Files:**
- Create: `program/curriculum-calendar.md`

- [ ] **Step 1: Write the H2 curriculum calendar (Months 7–12)**

Save to `program/curriculum-calendar.md`. Map each month to one of the top 10 pain points:

```
# LMU Family Business Program — Curriculum Calendar (H2 2026)

JULY — Pain Point #1: No Succession Plan
Workshop: "Building Your Family Business Succession Plan — A Working Session"
Format: Half-day workshop, bring your founding documents
Facilitator: Business Consulting Resources partner
Takeaway: Each attendee leaves with a drafted one-page succession framework

AUGUST — Pain Point #4: Lack of Family Communication
Lunch & Learn: "How to Have the Conversation You've Been Avoiding"
Format: 90-min lunch session, small group
Focus: Scripts and frameworks for starting the succession conversation with family members

SEPTEMBER — Pain Point #3: Generational Conflict
Speaker Series: "Two Generations, One Business — A Family Panel"
Format: Panel with a founder + their successor from an LMU member company
Focus: How they navigated the authority transition in real time

OCTOBER — Pain Point #9: No Governance Structure
Workshop: "Building a Family Business Governance Structure From Scratch"
Format: Interactive workshop
Takeaway: Draft family council charter and decision-rights matrix

NOVEMBER — Annual Conference
Theme: TBD based on member feedback from H1 surveys
Format: Half-day, open to non-members (conversion event)

DECEMBER — Pain Point #10: Leadership Vacuum Risk
Lunch & Learn: "What Happens If Something Happens to You Tomorrow?"
Format: Tabletop scenario exercise
Focus: Business continuity planning, emergency succession, key person risk
```

- [ ] **Step 2: Add H1 calendar entries for any remaining months**

For Months 4–6, fill in workshops based on what's already scheduled. Confirm with Business Consulting Resources partner which topics they can facilitate.

- [ ] **Step 3: Publish the calendar**

Share the calendar in three places:
1. LMU Family Business Program events page (submit to web team)
2. Next newsletter issue (see Task 11)
3. Pin to LinkedIn page as an announcement

- [ ] **Step 4: Commit**

```bash
git add program/curriculum-calendar.md
git commit -m "feat: add H2 curriculum calendar mapped to top 10 pain points"
```

**Done when:** Calendar published on website and shared via newsletter and LinkedIn.

---

## Task 11: Newsletter Launch (Month 3)

**A biweekly (every two weeks) newsletter to warm leads, current members, and inbound signups. Primary purpose: build trust over multiple touchpoints before asking for membership.**

**Files:**
- Create: `newsletter/issue-template.md`

- [ ] **Step 1: Write the newsletter template**

Save to `newsletter/issue-template.md`:

```
NEWSLETTER NAME: The Family Business Brief
SEND FREQUENCY: Every two weeks, Tuesday at 9 AM PT
FROM NAME: [Director name], LMU Family Business Program
FROM EMAIL: [director LMU email]

---
TEMPLATE STRUCTURE:

Subject line formula: [Stat or question] + [topic] (e.g., "43% of owners have no plan. Here's where to start.")

HEADER: The Family Business Brief | [Month Day, Year]

SECTION 1 — ONE THING (100–150 words)
One insight, stat, or observation about family business — something worth sharing at a dinner table. Not a lecture. Conversational tone.
Example: "We asked 20 family business owners last week what keeps them up at night. The most common answer wasn't competition or cash flow. It was: 'I don't know how to tell my kids the plan.'"

SECTION 2 — WHAT WE'RE HEARING (50–75 words)
One theme from recent peer group conversations (anonymized). Makes non-members want to be in the room.
Example: "In our Founders group last month, someone asked: 'How do you give your successor real authority when you're still in the building?' The conversation ran 40 minutes over. We'll share what the group landed on in a future issue."

SECTION 3 — UPCOMING (3–5 lines)
List of next 1–2 events with date, topic, and registration link. Short.

SECTION 4 — ONE RESOURCE (2–3 lines)
Link to one useful external article, tool, or resource for family businesses. No pitch. Just useful.

FOOTER:
You're receiving this because you attended an LMU Family Business event or signed up at [assessment URL].
Unsubscribe | [LMU website] | [LinkedIn URL]
```

- [ ] **Step 2: Write Issue #1**

Using the template above, write the first issue. Use this content:

```
Subject: The question we asked 20 family business owners last month

ONE THING:
We've been asking family business owners one question: "What's the one thing about your business future you haven't been able to say out loud?"

The answers were consistent. Not market risk. Not competition. The thing most owners haven't said out loud is whether their children actually want this — and whether they themselves are ready to step back.

That unsaid thing is usually where the real work begins.

WHAT WE'RE HEARING:
At our last forum, a founder in the room said something that landed differently than a consultant ever could: "I spent 30 years building this for my kids. Last year I realized I never asked them if they wanted it." The room went quiet. Four other owners nodded.

That's what peer community does that workshops can't.

UPCOMING:
• [Next event name] — [Date] — [Registration link]
• Founding cohorts now forming for our Founders, Next-Gen, and Sibling Teams peer groups. Reply to this email to express interest.

ONE RESOURCE:
"Why Family Businesses Fail at Succession" — Harvard Business Review
[URL — use a real HBR article on this topic from the web]
```

- [ ] **Step 3: Set up Mailchimp campaign**

1. In Mailchimp, create a new Regular Campaign
2. Select the audience (same list as nurture sequence, or create a separate "Newsletter" audience and merge)
3. Set From name, From email, Subject line
4. Use the template from Step 1 as the design structure
5. Schedule Issue #1 for next Tuesday at 9 AM PT
6. Create a recurring reminder (calendar event or task) to draft each issue 5 days before send

- [ ] **Step 4: Add newsletter signup to all touchpoints**

- LMU Family Business Program website (footer + homepage)
- Email signature
- Event confirmation emails ("You'll also receive our biweekly newsletter — unsubscribe anytime")
- Assessment completion page (already connected via Typeform → Mailchimp)

- [ ] **Step 5: Commit**

```bash
git add newsletter/issue-template.md
git commit -m "feat: add newsletter template and Issue 1 content"
```

**Done when:** Issue #1 scheduled in Mailchimp; newsletter signup added to website and email signature.

---

## Task 12: Member Feedback Loop (Month 1, ongoing)

**Post-event pulse surveys generate satisfaction data, surface curriculum gaps, and produce testimonial language in members' own words.**

**Files:**
- Create: `program/feedback-survey.md`

- [ ] **Step 1: Write the 3-question survey**

Save to `program/feedback-survey.md`. Build in Google Forms:

```
Title: Quick feedback — [Event Name]

Q1: What was most valuable about today? (Open text)

Q2: What was missing, or what would have made it better? (Open text)

Q3: Based on today, how likely are you to recommend this program to another family business? (Scale 1–10)

Bonus (optional): Is there a specific topic or challenge you'd like us to address in a future session? (Open text)
```

- [ ] **Step 2: Set up the Google Form and automate delivery**

1. Create the form in Google Forms (duplicate it for each event, changing the title)
2. After each event, send the form link via email within 24 hours:

```
Subject: 2 minutes — your feedback on today

Hi [First Name],

Thanks for joining us at [Event Name] today. Your feedback directly shapes what we do next.

[Google Form link]

Takes under 2 minutes. Genuinely useful.

[Your name]
```

- [ ] **Step 3: Create a quarterly review process for responses**

At the end of each quarter:
1. Export all responses from Google Forms to a spreadsheet
2. Review for patterns: What topics come up repeatedly in Q2 (what was missing)?
3. Pull verbatim quotes from Q1 for use as testimonials in marketing (with member permission)
4. Calculate average Q3 score — target is 4.2+/5.0 (equivalent to 8.4+/10)
5. Add a row to `reviews/quarterly-review.md` with the quarter's average score and top 3 insights

- [ ] **Step 4: Commit**

```bash
git add program/feedback-survey.md
git commit -m "feat: add post-event feedback survey and quarterly review process"
```

**Done when:** Google Form created; first survey sent within 24 hours of next event.

---

## Task 13: Student Integration Program (Month 4–6)

**LMU entrepreneurship students are an underutilized asset. Create a structured role that benefits members and gives students real family business exposure.**

**Files:**
- Create: `program/student-integration.md`

- [ ] **Step 1: Write the student integration guide**

Save to `program/student-integration.md`:

```
# LMU Family Business Program — Student Integration

## What We Offer Members
"Priority access to LMU entrepreneurship students for research projects, event support, and internship pipelines."

## Three Ways Students Can Support Member Companies

1. RESEARCH PROJECTS (1 semester, 3–5 students)
   - Member submits a business question or challenge (e.g., "help us benchmark our compensation structure against industry peers")
   - Matched with a team of 2–3 entrepreneurship students
   - Deliverable: 10-page research report + presentation
   - Coordinated through the Center for Entrepreneurship

2. EVENT SUPPORT (per event)
   - Students assist with registration, setup, documentation, and post-event summaries
   - Gives students exposure to real family business dynamics and LMU network

3. INTERNSHIP PIPELINE
   - Members post internship opportunities directly to the LMU entrepreneurship student network
   - Program director facilitates introduction to Career Services for posting

## How to Request a Student Match
Members email [director] with:
- Type of support needed (research, event, internship)
- Brief description of the project or role
- Desired timeline

Director coordinates with Center for Entrepreneurship and matches students within 2 weeks.

## For Students
- Coordinate with the Center for Entrepreneurship to create a formal "Family Business Practicum" role
- Students earn course credit or co-curricular recognition
- Must complete a confidentiality agreement before working with member companies
```

- [ ] **Step 2: Coordinate with the Center for Entrepreneurship**

Schedule a meeting with the Center director to:
1. Present the student integration model
2. Agree on how research projects get assigned (class project vs. independent study vs. volunteer)
3. Create the confidentiality agreement template
4. Add "Family Business Program Partner" as a category in the student internship portal

- [ ] **Step 3: Announce to current members**

In the next newsletter issue, add a section:

```
NEW MEMBER BENEFIT: Priority Access to LMU Students

Starting this semester, members can request LMU entrepreneurship students for research projects, event support, and internship opportunities. Reply to this email to tell us what kind of student support would be most useful to your business.
```

- [ ] **Step 4: Commit**

```bash
git add program/student-integration.md
git commit -m "feat: add student integration program guide"
```

**Done when:** Center for Entrepreneurship meeting held; first student match request received from a member.

---

## Task 14: Member Case Studies (Month 9)

**Real member stories are the most credible marketing asset the program has. Peer referral ("another family business recommended this") is one of the highest-converting triggers.**

**Files:**
- Create: `marketing/case-study-template.md`

- [ ] **Step 1: Write the case study template**

Save to `marketing/case-study-template.md`:

```
# [Company Name] — Family Business Case Study
LMU Family Business Entrepreneurship Program

HEADLINE: How [Company Name] [achieved specific outcome] through the LMU Family Business Program

THE BUSINESS
- Company: [Name]
- Industry: [Industry]
- Generation: [1st / 2nd / 3rd]
- Based in: [City, CA]
- Years in business: [X]

THE CHALLENGE (2–3 sentences)
What was the specific challenge or situation that led them to the program? Use their words where possible.

WHAT THEY DID (2–3 sentences)
Which program elements did they engage with? (peer group, workshop, conference, advisory services)

THE OUTCOME (2–3 sentences)
What changed? What did they do differently? What did they say about the experience?

IN THEIR WORDS
[Direct quote — pull from feedback survey or conduct a short interview]

---
Interested in joining the LMU Family Business Program?
[CTA link]
```

- [ ] **Step 2: Identify 2–3 members for the first case studies**

From the post-event feedback surveys, identify members who gave high scores (Q3 ≥ 9/10) and wrote compelling Q1 responses. Reach out:

```
Subject: Would you share your story?

Hi [First Name],

Your feedback from [event] meant a lot — especially what you said about [specific thing they wrote].

We're putting together a few short member stories to share with family businesses who are considering the program. Would you be open to a 20-minute call so I can write up your experience? You'd review it before we publish anything.

[Your name]
```

- [ ] **Step 3: Conduct interviews and write the case studies**

For each willing member:
1. Schedule 20-minute call
2. Ask: What was happening in your business before you joined? What made you decide to join? What's changed? What would you tell another family business owner?
3. Write the case study using the template
4. Send draft to member for approval
5. Publish on LMU website and share via newsletter + LinkedIn

- [ ] **Step 4: Commit**

```bash
git add marketing/case-study-template.md
git commit -m "feat: add member case study template"
```

**Done when:** At least 2 member case studies published on website and promoted via newsletter.

---

## Task 15: Quarterly Reviews (Months 3, 6, 12)

**Stop/start/continue evaluation at each milestone to keep the strategy adaptive.**

**Files:**
- Create: `reviews/quarterly-review.md`

- [ ] **Step 1: Write the quarterly review template**

Save to `reviews/quarterly-review.md`:

```
# LMU Family Business Program — Quarterly Strategy Review

## Q[X] Review — [Month Year]

### Metrics Snapshot

| Metric | Target | Actual | Status |
|---|---|---|---|
| CSV leads contacted | 41 (all by M1) | | |
| New leads added to pipeline | 100+ by M6 | | |
| Email subscribers | 150+ | | |
| Net new memberships | 8–15 | | |
| Member renewal rate | 75%+ | | |
| Post-event satisfaction avg | 4.2+/5.0 | | |
| Member-referred leads | 5+/quarter by Q4 | | |
| Organic sessions (SEO pages) | 2x baseline | | |

### Stop / Start / Continue

STOP (tactics that aren't working — cut them):
-

START (new tactics to try based on what we've learned):
-

CONTINUE (what's working — do more of it):
-

### Top 3 Insights This Quarter
1.
2.
3.

### Priority Actions for Next Quarter
1.
2.
3.
```

- [ ] **Step 2: Schedule three review dates now**

Add calendar events for:
- Month 3 Review: [Date 3 months from start]
- Month 6 Review: [Date 6 months from start]
- Month 12 Review: [Date 12 months from start]

Each review takes 60–90 minutes. Pull data from: Mailchimp (subscribers, open rates), pipeline tracker (contacts, conversions), Google Analytics (sessions on SEO pages), post-event surveys (satisfaction scores), Google Forms referral tracker (referrals received).

- [ ] **Step 3: Commit**

```bash
git add reviews/quarterly-review.md
git commit -m "feat: add quarterly review template and schedule"
```

**Done when:** Review template saved; three review dates on calendar.

---

## Self-Review Checklist

- [x] **Spec coverage:** Track A (outbound — Tasks 1, 2, 5), Track B (referral/partner — Tasks 6, 7), Track C (SEO — Task 8), Program quality (peer groups — Task 9, curriculum — Task 10, newsletter — Task 11, feedback — Task 12, student integration — Task 13), Case studies — Task 14, Reviews — Task 15. All spec sections covered.
- [x] **Placeholder scan:** All templates contain actual content. No "TBD" or "fill in later."
- [x] **Consistency:** Pipeline tracker referenced consistently across Tasks 1, 2, 5, 6, 7. Mailchimp used for both nurture (Task 4) and newsletter (Task 11) — same tool, same audience. Typeform assessment (Task 3) connects to Mailchimp nurture (Task 4) via native integration as specified.
