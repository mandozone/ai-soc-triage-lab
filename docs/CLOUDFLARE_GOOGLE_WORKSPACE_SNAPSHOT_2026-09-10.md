# Mando Corporation — Cloudflare + Google Workspace Snapshot

**Snapshot date:** 2026-09-10

## Purpose
This file records the Cloudflare, website, and Google Workspace/email configuration work completed for `mandocorporation.com` through Sep 10, 2026. It is intended as the canonical recovery/reference snapshot for future troubleshooting.

## Current live domain state
- Domain: `mandocorporation.com`
- Cloudflare live/authoritative zone identified and confirmed.
- Live nameservers:
  - `mira.ns.cloudflare.com`
  - `melnicoff.ns.cloudflare.com`
- A duplicate/pending Cloudflare zone was also discovered using different nameservers (`riya.ns.cloudflare.com` / `trey.ns.cloudflare.com`). Do **not** switch nameservers to the pending zone.
- Website/Worker/nameserver configuration was intentionally left unchanged during email migration.

## Website deployment / GitHub
- Repository: `mandozone/ai-soc-triage-lab`
- Website branch: `mando-corporation-site`
- Cloudflare Worker name in `wrangler.jsonc`: `mando-corporation`
- Static asset directory: `./public`
- Website source served from `public/index.html`
- Public website contact email updated from `partnership@mandocorporation.com` to `sales@mandocorporation.com`.
- Update commit: `12563f1dd464cf8008de0e00cb279acfd29af500`
- Both footer contact text and Ask Mando `mailto:` contact route were updated.

## Google Workspace account
- Workspace created for Mando Corporation.
- Primary business mailbox: `sales@mandocorporation.com`
- Display/user name: Romando Wright
- Business Starter plan selected.
- Domain verification completed successfully through Cloudflare.
- Google verification TXT record was authorized through the correct Cloudflare zone.

## Cloudflare Email Routing migration
### Previous state
Cloudflare Email Routing was previously handling inbound mail and had created these MX records:
- `route1.mx.cloudflare.net`
- `route2.mx.cloudflare.net`
- `route3.mx.cloudflare.net`

It also had Cloudflare-specific SPF/DKIM records, including an old DKIM selector at:
- `cf2024-1._domainkey.mandocorporation.com`

### Migration completed
- Cloudflare Email Routing disabled.
- Old Cloudflare MX records removed.
- Old Cloudflare DKIM record removed after Google DKIM was active.
- Old Cloudflare SPF authorization removed/replaced.

## Current Google Workspace DNS / mail authentication
### MX
- Active root MX: `smtp.google.com`
- Priority: `1`
- TTL: Auto
- No other root MX records should remain.

### SPF
Exactly one root SPF TXT record:

`v=spf1 include:_spf.google.com ~all`

### DKIM
- Google Workspace DKIM enabled.
- 2048-bit Google DKIM key published.
- Google Admin authentication started/active.
- Controlled test showed DKIM PASS.

### DMARC
DMARC TXT record added at `_dmarc.mandocorporation.com` with monitoring policy:

`v=DMARC1; p=none;`

This is intentionally cautious while sender reputation is being established.

## Verification results
A controlled Gmail test from `sales@mandocorporation.com` showed:
- SPF: PASS
- DKIM: PASS
- DMARC: PASS
- Public DNS: verified
- Gmail activation: YES

One early authenticated test landed in Spam, but subsequent simple messages from `sales@mandocorporation.com` landed in Inbox, including normal conversational traffic and a reply thread.

## Sender / outreach operating rules
### International outreach
Use:
- `sales@mandocorporation.com`

Primary offer:
- managed international U.S.-market-entry campaigns
- digital billboards + Hulu/Disney+ / CTV when appropriate

### U.S. local niche outreach
Use:
- `mandocorporation5@gmail.com`

Typical local niches:
- HVAC
- roofing
- auto
- construction
- med spa
- legal
- other high-ticket local services

### Deliverability rules
- Verify sender before every send.
- Never guess prospect email addresses.
- Official company website/contact route first.
- No retries to bounced or blocked addresses.
- No large volume spikes on the new Workspace mailbox.
- Warm `sales@mandocorporation.com` gradually with legitimate conversations and low-volume personalized outreach.
- Report delivery status using:
  - `BOUNCED/REJECTED`
  - `SENT — NO FAILURE DETECTED`
  - `REPLIED`
- Do not claim inbox placement unless actually verified.

## Historical issue to avoid
`mandocorporation5@gmail.com` developed poor cold-outreach reputation after heavy sending, bounces, recipient blocks, and at least one test that Gmail placed in Spam with a warning that the message resembled prior spam. It should not be used for international/primary outbound growth campaigns going forward.

## Important do-not-change items
Unless specifically required and verified:
- Do not change Cloudflare nameservers.
- Do not modify unrelated DNS.
- Do not alter the `mando-corporation` Worker while troubleshooting email.
- Do not edit website A/CNAME records as part of mail work.
- Do not recreate Cloudflare Email Routing unless intentionally abandoning Google Workspace inbound mail.
- Do not create or use the duplicate pending Cloudflare zone.

## Recovery checklist
If mail breaks in the future, verify in this order:
1. Public nameservers are still `mira.ns.cloudflare.com` and `melnicoff.ns.cloudflare.com`.
2. Root MX points only to `smtp.google.com` with priority 1.
3. Exactly one SPF root record exists: `v=spf1 include:_spf.google.com ~all`.
4. Google DKIM selector resolves and Google Admin shows authentication active.
5. `_dmarc` resolves to `v=DMARC1; p=none;` (or any later intentionally upgraded policy).
6. Cloudflare Email Routing remains disabled.
7. Send one controlled test and inspect SPF/DKIM/DMARC results before changing anything else.

## Current status
- Google Workspace migration: COMPLETE
- Gmail activated: YES
- SPF: PASS
- DKIM: PASS
- DMARC: PASS
- Cloudflare Email Routing: DISABLED
- Website contact updated to `sales@mandocorporation.com`
- Ready for high-volume outreach: NO — sender reputation is still being established
