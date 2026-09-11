# Mando Corporation — Comprehensive Operating Snapshot

**Snapshot date:** 2026-09-10  
**Latest operating update:** 2026-09-11  
**Repository:** `mandozone/ai-soc-triage-lab`  
**Website branch:** `mando-corporation-site`  
**Website:** `mandocorporation.com`

---

## 1. Company Positioning

Mando Corporation is positioned as a managed advertising partner focused on geographically targeted campaigns. The operating model started with digital out-of-home (DOOH) / digital billboard campaigns and expanded into a hybrid advertising model combining:

- Digital billboards / DOOH
- Premium streaming TV / CTV, especially Hulu and Disney+
- OOH-only, CTV-only, or coordinated hybrid campaigns
- Market planning
- Geographic targeting
- Creative adaptation / production coordination
- Placement / activation coordination
- Campaign reporting and delivery summaries

The client-facing value proposition is not simply “selling a billboard.” The stronger positioning is: define the business objective, identify the right market and traffic corridors, shape the media plan, adapt creative, coordinate placement, and report delivery through one managed relationship.

No campaign should be represented as guaranteeing leads, sales, ticket sales, or ROI.

---

## 2. Core Operating Doctrine

### Broad intelligence, narrow execution

Mando should scan widely for commercial signals but execute only where there is a clear reason to buy media.

The durable sequence is:

**SCAN → DETECT → FILTER → MATCH INVENTORY → RESEARCH → VERIFY → SCORE → CHECK ECONOMICS → OUTREACH → TRACK → LEARN**

A related buyer-path version is:

**Signal → Buyer → Verified contact → Outreach → Response → Inventory → Proposal → Payment → Launch → Report**

### Evidence over optimism

Prioritize prospects with visible evidence of:

- U.S. expansion
- retail distribution
- new market entry
- launches
- openings
- events / festivals / tours
- release dates
- sponsorship activity
- distribution deals
- promotional momentum
- geographic expansion
- timing windows where visibility matters

### One-prospect-at-a-time execution

Mando’s strongest outreach workflow is individualized and sequential rather than indiscriminate bulk sending.

Core principle: **do not pad volume with guessed or weak contacts.**

---

## 3. Prospecting Engines

### A. Local high-ticket services

Priority local niches include:

- HVAC
- Roofing
- Plumbing
- Electrical
- Construction / home improvement
- Auto repair / body shops
- Legal
- Med spa / aesthetics
- Gyms / fitness
- Apartment / leasing
- Pool services
- Other local services where one converted customer can justify meaningful ad spend

Restaurants are excluded from the preferred local workflow.

### B. Entertainment intelligence

Track and prospect around:

- Film releases
- Streaming launches
- TV premieres
- Music releases
- Tours
- Festivals
- Theater / Broadway
- Comedy
- Gaming / esports
- Production companies
- Distributors
- Studios
- Labels
- Agencies
- Promoters
- Awards campaigns

### C. Ad-spend / expansion intelligence

Look for companies actively spending, launching, expanding, distributing, sponsoring, or entering new regions.

### D. Calendar intelligence

Maintain a forward-looking 30 / 60 / 90-day view of known commercial moments, including:

- entertainment launches
- tours
- festivals
- conventions
- seasonal demand
- store openings
- retail launches
- product launches
- company expansion
- construction / infrastructure milestones
- sporting events
- other scheduled events that may trigger advertising demand

### E. International market-entry intelligence

Priority international categories include:

1. International food / beverage brands entering the U.S.
2. Foreign CPG brands gaining U.S. retail distribution
3. Films, music, tours, and entertainment entering U.S. markets
4. Foreign retailers opening U.S. stores
5. Travel / tourism brands
6. International apps / technology firms entering the U.S.
7. Beauty brands with a strong retail or expansion trigger
8. B2B only when the trigger and buyer fit are strong

International pitch framing should emphasize **U.S. market-entry media campaigns**, not just “billboards.”

---

## 4. Outreach Contact Verification Rules

This is a core rule and should not be bypassed.

### Required order

1. Official company website first
2. Find the exact published marketing / partnerships / business-development / press / contact route
3. Verify the email address or contact form from first-party sources
4. Check Mando’s Gmail history for duplicates, previous outreach, bounces, suppressions, or replies
5. Research the company trigger and buyer context
6. Personalize the subject and opening
7. Send from the correct sender lane
8. Track the response / failure status

### Never do this

- Do not guess email patterns
- Do not use speculative first-name.last-name addresses without verification
- Do not retry known hard bounces
- Do not retry recipient-blocked addresses without a new verified route
- Do not treat “sent” as proof of inbox placement
- Do not call no-bounce delivery “successful”

### Reporting statuses

Use:

- **BOUNCED / REJECTED** — confirmed non-delivery
- **SENT — NO FAILURE DETECTED** — no bounce seen, inbox placement unknown
- **REPLIED** — confirmed engagement
- **NOT SENT — ACCOUNT LIMIT / ERROR** — message never left the sender account

---

## 5. Sender Account Strategy

### Current sender split

#### International outreach

Use:

**`sales@mandocorporation.com`**

Primary use:

- international companies
- U.S. market-entry campaigns
- digital billboard + Hulu / Disney+ hybrid pitch
- larger brands / launches / entertainment / retail expansion

#### Local U.S. niche outreach

Use:

**`mandocorporation5@gmail.com`**

Primary use:

- local HVAC
- roofing
- auto
- construction
- med spa
- legal
- other local U.S. service niches

### Historical mailbox rule

`mandocorporation5@gmail.com` should not be deleted because it contains:

- outreach history
- prospect replies
- bounces
- suppression information
- pipeline context
- old snapshots
- historical intelligence

---

## 6. Deliverability Incident and Lessons

The legacy sender `mandocorporation5@gmail.com` experienced substantial deliverability problems after high-volume outreach.

Observed failure classes included:

- Gmail account sending-limit failures
- recipient-side message blocked / rejected responses
- address-not-found hard bounces
- spam placement

A controlled test to a Gmail recipient showed the warning:

> “This message is similar to messages that were identified as spam in the past.”

This confirmed that the old Gmail sender had developed a spam-reputation / content-pattern problem.

### Durable lessons

- Sender reputation matters as much as recipient verification
- High-volume cold outreach from one consumer Gmail account is unsafe
- Repeated / near-identical copy can damage placement
- Hard-bounce suppression must be permanent unless a new first-party contact route is found
- Volume should be ramped gradually
- Reply activity and legitimate two-way conversations are useful for warming a new mailbox
- Inbox placement must be measured through controlled tests, not assumed from a lack of bounce

---

## 7. New Google Workspace Mailbox

### Active business mailbox

**`sales@mandocorporation.com`**

Google Workspace was successfully created and configured.

The mailbox is a real outbound Gmail / Workspace user and is connected to ChatGPT as a separate Gmail connection.

### Current authentication state

As of this snapshot:

- Gmail activated: **YES**
- Google MX is active
- SPF passes
- Google DKIM passes
- DMARC passes
- Public DNS was verified
- Cloudflare Email Routing was disabled
- Controlled tests showed mixed early reputation behavior: one test initially landed in Spam, later simple human-style messages landed in Inbox

### Warm-up principle

Treat `sales@mandocorporation.com` as a new sender identity.

Initial activity should favor:

- short normal emails
- genuine two-way replies
- limited sending volume
- low bounce rate
- no sudden spikes
- no mass-copy template behavior

Ramp only after repeated clean inbox placement.

---

## 8. Google Workspace / Cloudflare Mail Configuration

### Domain

`mandocorporation.com`

### Live authoritative Cloudflare nameservers

- `mira.ns.cloudflare.com`
- `melnicoff.ns.cloudflare.com`

A duplicate / pending Cloudflare zone was discovered using different nameservers:

- `riya.ns.cloudflare.com`
- `trey.ns.cloudflare.com`

**Do not change production nameservers to the pending duplicate zone.**

### Cloudflare Email Routing

Cloudflare Email Routing previously handled inbound forwarding and created managed mail DNS records.

It was disabled as part of the Google Workspace migration.

Historical Cloudflare MX records removed from the live zone:

- `route1.mx.cloudflare.net`
- `route2.mx.cloudflare.net`
- `route3.mx.cloudflare.net`

### Google Workspace MX

The domain was migrated to Google Workspace mail handling.

Google’s setup used:

- Type: MX
- Host: `@`
- Priority: `1`
- Target: `smtp.google.com`

### SPF

Historical Cloudflare forwarding SPF:

`v=spf1 include:_spf.mx.cloudflare.net ~all`

Current Google Workspace SPF:

`v=spf1 include:_spf.google.com ~all`

Rule: exactly one SPF TXT record at the root.

### DKIM

Google Workspace 2048-bit DKIM was generated, published in Cloudflare, and authentication was started in Google Admin.

The old Cloudflare Email Routing DKIM record at `cf2024-1._domainkey` was legacy infrastructure and not part of the new Google Workspace sender authentication.

### DMARC

DMARC was added at:

`_dmarc.mandocorporation.com`

Initial policy:

`v=DMARC1; p=none;`

This is intentionally cautious during warm-up and monitoring.

### Authentication verification

Controlled test results confirmed:

- SPF = PASS
- DKIM = PASS
- DMARC = PASS

---

## 9. Cloudflare Safety Rules

When modifying Cloudflare for Mando email work:

### Do not touch

- website content unless explicitly requested
- Worker unrelated settings
- Pages unrelated settings
- nameservers
- A records unrelated to mail
- CNAME records unrelated to mail
- unrelated TXT records
- unrelated DNS

### Mail-change order

1. Identify active Cloudflare zone
2. Confirm live nameservers
3. Confirm current mail provider
4. Remove conflicting old routing records only
5. Add / verify new provider MX
6. Configure SPF
7. Configure DKIM
8. Configure DMARC
9. Verify public DNS
10. Send controlled tests
11. Inspect message headers
12. Only then begin warm-up / outreach

---

## 10. Website / GitHub / Cloudflare Deployment

### GitHub repository

`mandozone/ai-soc-triage-lab`

### Mando website branch

`mando-corporation-site`

This branch contains the Mando Corporation website and should not be confused with the cybersecurity project on `main`.

### Wrangler config

The Mando Cloudflare deployment serves the `./public` directory.

Worker / app name:

`mando-corporation`

### Website source

Primary live-site source:

`public/index.html`

### Website contact email

Website public contact email was updated from:

`partnership@mandocorporation.com`

to:

`sales@mandocorporation.com`

The change covered:

- visible footer email
- Ask Mando contact response
- `mailto:` link

The update was committed on 2026-09-10 with commit:

`12563f1dd464cf8008de0e00cb279acfd29af500`

### Existing Cloudflare / Google Workspace snapshot

A separate configuration snapshot already exists at:

`docs/CLOUDFLARE_GOOGLE_WORKSPACE_SNAPSHOT_2026-09-10.md`

Commit:

`f26b54821fcecdd38803b43eaad6cddc723583a8`

---

## 11. Website Positioning / UX

Current website positioning emphasizes:

- managed digital billboard campaigns
- strategy
- creative
- activation
- reporting
- one point of contact

Current core campaign lanes shown on the site include:

- Local High-Ticket
- Event Amplification
- Brand Launches

The website includes:

- industry imagery
- local business examples
- campaign process
- pricing examples
- contact form
- “Ask Mando” lightweight website assistant

Current pricing displayed on the website includes:

- Launch — 2-week local test — **$750**
- Growth — 2-week stronger exposure — **$1,200**
- Established — 2-week higher-exposure local campaign — **$2,500**
- Brand / entertainment / event / multi-market — custom proposal

Historical Mando pricing also included a later monthly target of **$2,000/month** for some local proposals. Pricing should always be matched to the current campaign model and verified underlying media economics before quoting.

**Pricing status note (2026-09-11):** the website figures above are legacy display examples and are not the authoritative Hulu / Disney+ streaming or billboard-plus-streaming package prices. The active package prices are locked in Section 13. The public website was not changed by this snapshot-only update.

---

## 12. Inventory / Geography Rules

### Board-first doctrine

A durable rule is:

**Look up the board / inventory first before pitching a local prospect whenever possible.**

The intended sequence:

1. Find inventory
2. Check location and corridor
3. Review economics
4. Approve market fit
5. Prospect businesses that benefit from that geography
6. Outreach with a location-specific reason

### Newark cluster historical reference

Known Newark-area inventory references included:

- Route 21 / Harrison / McCarter Highway
- I-78 / Route 9
- I-280 interchange

Historical board cost reference discussed:

- about **$18/day**

Historical Newark delivery estimate:

- about **847–1,200 plays/month**
- about **44.8K–64K impressions/month**

Two-week equivalent:

- about **425–600 plays**
- about **22K–32K impressions**

Newark pitch rule: emphasize **reach**, not inflated play counts.

Example framing:

> “Your ad reaches an estimated 44–64 thousand views a month on a board right on McCarter Highway.”

Do not reuse Fairfield-type 3,000+ play figures for Newark inventory.

---

## 13. Campaign Economics

### Authoritative package pricing — locked 2026-09-11

The following prices are the current active Mando prices for Hulu / Disney+ streaming and coordinated billboard-plus-streaming campaigns:

- **Streaming Pilot — $1,500/month**
  - Planning media allowance: approximately **$500**
  - Planning gross margin: approximately **$1,000** before production, labor, taxes, and operating expenses
- **Streaming Growth — $2,500/month**
  - Planning media allowance: approximately **$1,000**
  - Planning gross margin: approximately **$1,500** before production, labor, taxes, and operating expenses
- **Billboard + Streaming — $4,000/month**
  - Planning underlying media cost: approximately **$1,040** when using the historical Newark board reference of about $18/day plus a $500 streaming campaign
  - Planning gross margin: approximately **$2,960** before production, labor, taxes, and operating expenses
- **Video production — $500–$750 one-time when needed**
  - Charge separately when the client does not already have an approved 15–30 second video creative

These prices supersede conflicting older package prices for these specific streaming and hybrid offers. Do not change them without a newer explicit instruction from the user.

The streaming media figures are planning allowances, not guaranteed final costs. Before sale or launch, confirm the selected platform, geography, dates, targeting, inventory, forecast, creative requirements, and actual media cost. Approved external language remains: **“Hulu, Disney+, and other premium streaming inventory, subject to platform availability and approval.”**

Before quoting any client:

- check real media cost
- check campaign duration
- check placement / inventory availability
- confirm projected delivery
- preserve Mando margin
- do not quote from stale estimates

Illustrative historical model:

- client pays $8,500
- media cost $5,000
- other costs $500
- gross profit about $3,000

This is an example only, not a default proposal.

Historical creator campaign structure:

- $750 — upcoming / smaller
- $1,200 — growing / decent
- $2,500 — established
- custom monthly pricing as needed

---

## 14. Streaming / CTV Strategy

### Disney / Hulu

Disney Campaign Manager was identified as the easiest current self-service / agency-friendly route for CTV campaigns involving Hulu / Disney+ inventory.

Mando pitch language may say that campaigns can include Hulu / Disney+ when appropriate, but must not imply affiliation with Disney or guaranteed inventory.

Do not promise:

- exact shows
- exact platform placement
- exact impression counts
- guaranteed delivery

until forecast / approval exists.

Use **impressions**, not “views,” for CTV reporting.

### Netflix

Netflix was discussed as premium inventory generally bought programmatically through DSPs such as:

- DV360
- Amazon DSP
- Yahoo DSP
- The Trade Desk

No simple self-service equivalent was confirmed for Mando at the time of research.

---

## 15. Outreach Message Structure

For strong cold outreach:

### Subject

Make the media proposition obvious when relevant.

Examples:

- Digital Billboards + Hulu/Disney+
- U.S. launch campaign idea
- Market-specific billboard + streaming plan

### Opening

Lead with the trigger:

- new U.S. launch
- expansion
- retail rollout
- opening
- tour
- release
- event
- distribution

### Body

Explain why the campaign fits their geography and timing.

### Close

Offer a short market-specific concept / rollout plan.

Do not lead cold outreach with payment links.

Payment link comes after interest / campaign selection.

---

## 16. Current Tool / Integration Map

### Gmail

Connected mailboxes:

- `mandocorporation5@gmail.com`
- `sales@mandocorporation.com`

### GitHub

Used for:

- website source
- Mando snapshots
- deployment-related source files

### Cloudflare

Used for:

- domain
- DNS
- website / Worker deployment
- mail DNS authentication

### Stripe

Used for:

- payment links / proposal payment flow

### Call-E

Used for:

- test calls
- sales-call scripting
- phone outreach experiments

### LinkedIn / Indeed / GitHub career tooling

Also used separately for recruiting / job-search workflows and should remain separate from Mando operational changes unless explicitly requested.

---

## 17. Pipeline / Follow-up Conventions

Use clear prospect statuses such as:

- ACTIVE FOLLOW-UP
- SENT / AWAITING REPLY
- WAITING ON EMAIL RESPONSE
- CALLBACK
- PENDING PARTNER REVIEW
- CLOSED / NOT INTERESTED
- LEFT VOICEMAIL
- NO ANSWER
- NOT IN SERVICE

Historical examples:

- RK Roofing — active follow-up
- Above & Beyond Plumbing & Heating — waiting on email response
- Masonry Pro Construction — closed / not interested
- Joe Cardoso — closed / not interested
- LGM Roofing — sent / awaiting reply
- Don Pepe — callback status at the time
- Paper Flowers / Asit Vyas — substantive engagement and later pass due timing

Do not revive closed / not-interested prospects unless they re-engage.

---

## 18. Daily Workflow and Volume Philosophy

Historical aspirational volume targets reached as high as 100/day across intelligence engines, but deliverability events showed that volume cannot override sender quality.

Current rule:

**quality and deliverability come before volume.**

For a new authenticated mailbox:

- begin with normal conversations
- build two-way reply history
- send low-volume highly qualified outreach
- increase only after clean inbox placement
- do not jump immediately to hundreds per day from one fresh sender

---

## 19. Known Deliverability Suppression Examples

Historical blocked / rejected or dead recipients included examples such as:

- eastorange@puregym.com
- boston@thehawksmoor.com
- service@aritzia.com
- sponsorship@abffventures.com
- Inquiries@gongchausa.com
- global.sales@dreame.tech
- sales@develeyusa.com
- info@nongshimusa.com
- hey@whateverbrands.com
- global@torriden.com
- hello@jenvi.com
- Social@bondiboost.com
- contact@hyh-america.com
- btminy@visitbarbados.org
- candelaplumbing@gmail.com
- espinolatech@yahoo.com
- info@biggerandbetterthangs.com
- info@swanaestheticsatl.com
- info@amariaesthetic.com

These are historical suppression examples. Do not automatically retry them. Only reconsider if a new, verified first-party route is found.

---

## 20. Current Sender-Routing Rule

This rule should be treated as authoritative until changed explicitly:

### International / larger expansion campaigns

Send from:

**`sales@mandocorporation.com`**

Primary pitch:

**Digital billboards + Hulu / Disney+**

### Local U.S. niche campaigns

Send from:

**`mandocorporation5@gmail.com`**

Primary pitch:

local billboard / local campaign fit based on geography and service area.

Always verify sender before sending.

---

## 21. Recovery / Troubleshooting Checklist

If email or website configuration breaks again:

### Website

1. Check `mandozone/ai-soc-triage-lab`
2. Use branch `mando-corporation-site`
3. Confirm `wrangler.jsonc`
4. Confirm assets directory is `./public`
5. Confirm `public/index.html` is the live source
6. Do not edit cybersecurity content on `main`

### Cloudflare

1. Confirm active zone is `mandocorporation.com`
2. Confirm nameservers are `mira.ns.cloudflare.com` and `melnicoff.ns.cloudflare.com`
3. Do not use the duplicate `riya/trey` pending zone
4. Do not change nameservers without a separately approved migration plan

### Gmail / Workspace

1. Confirm `sales@mandocorporation.com` can sign in
2. Confirm MX is Google
3. Confirm exactly one SPF record
4. Confirm Google DKIM authentication is active
5. Confirm DMARC exists
6. Send controlled test
7. Inspect SPF / DKIM / DMARC headers
8. Check Inbox / Promotions / Spam placement

---

## 22. Snapshot Priority Rule

When newer instructions conflict with older historical snapshots, **the newest explicit operating instruction wins**.

Historical snapshots should be preserved as evidence and context, but current sender rules, current pricing, current deployment configuration, and current campaign positioning supersede older states.

---

## 23. Current Known-Good State — 2026-09-10

- `mandocorporation.com` remains the Mando website and business domain
- `sales@mandocorporation.com` is the active Google Workspace business mailbox
- Google Workspace mail authentication is passing SPF / DKIM / DMARC
- Cloudflare Email Routing is disabled
- live Cloudflare nameservers remain `mira.ns.cloudflare.com` / `melnicoff.ns.cloudflare.com`
- Mando website source lives on `mando-corporation-site`
- `public/index.html` is the live website source
- website public email is `sales@mandocorporation.com`
- international outreach uses `sales@mandocorporation.com`
- local U.S. niche outreach uses `mandocorporation5@gmail.com`
- international campaigns are positioned as U.S. market-entry media opportunities, often combining digital billboards + Hulu / Disney+
- active package pricing is $1,500/month Streaming Pilot, $2,500/month Streaming Growth, and $4,000/month Billboard + Streaming; video production is $500–$750 one-time when needed
- recipient verification must come from first-party sources before sending
- sender identity must be explicitly checked before each send
- deliverability health takes priority over raw outreach volume

---

## 24. Git Commit References

- Website contact-email update: `12563f1dd464cf8008de0e00cb279acfd29af500`
- Cloudflare / Google Workspace snapshot: `f26b54821fcecdd38803b43eaad6cddc723583a8`
- This comprehensive snapshot commit: created by the commit that adds this file

---

**End of snapshot.**
