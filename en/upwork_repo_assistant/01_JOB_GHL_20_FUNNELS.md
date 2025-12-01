# JOB ADD-ON – Setup GoHighLevel Domain + Connect It With 20 Funnels (Based on Paths)

This add-on sits on top of the Universal Header and is specifically for an Upwork job where the client wants **one root domain configured in GoHighLevel** and mapped to **~20 funnels, each with its own path** (e.g. `/events`, `/training`, `/apply`).

## Extra repo artefacts

In addition to the standard files, create these extra Markdown files inside the job folder:

1. `09_ghl_routing_matrix.md`

   - Table with columns:
     - `Path`
     - `Funnel / Funnel Step`
     - `Intended Use (events, training, apply, etc.)`
     - `Primary CTA`
     - `Status` (planned / configured / tested)
     - `Notes`
   - Prepopulate ~20 placeholder rows with generic paths (e.g. `/events`, `/training`, `/apply`, `/lead-magnet-1`, `/webinar-1`, `/onboarding`, `/thank-you-1`, `/upsell-1`, etc.) that I can later edit to match the real funnel names.

2. `10_dns_ssl_plan.md`

   - Sections:
     - `# DNS & SSL Plan`
     - `## Current Assumptions`
     - `## DNS Records To Configure`
     - `## Zero-Downtime Strategy`
     - `## SSL & Verification Steps`
     - `## Post-GoLive Checks`
   - List the typical A/CNAME record patterns for connecting a root or subdomain to GoHighLevel, but clearly mark anything that depends on the registrar/host as **TO CONFIRM WITH CLIENT**.

3. `11_test_plan_routing.md`
   - Sections:
     - `# Routing & QA Test Plan`
     - `## Desktop Tests`
     - `## Mobile Tests`
     - `## Edge-Case Tests`
   - Include explicit checks for:
     - wrong/typo paths
     - 404 / default behaviour
     - conflicts between funnels sharing similar paths
     - HTTP → HTTPS redirects
     - `www` vs bare domain behaviour (if applicable).

## Customisations to the standard artefacts

When generating the standard files, bias them towards **domain + routing architecture** work rather than funnel copy/design.

### Requirements Snapshot

- Emphasise:
  - Single domain → multiple GHL funnels via path routing.
  - Clean, conflict-free path strategy (no overlap, no duplicate root paths).
  - Proper DNS & SSL configuration with verification.
  - Cross-device behaviour (desktop & mobile).
- Under “Implied / Hidden Work”, explicitly include:
  - Time for DNS propagation and verification issues.
  - Backup/rollback plan in case the domain is currently serving a live site elsewhere.
  - Documentation so the client (or their team) can add future funnels safely.

### Solution Outline

- Structure the solution into **four phases**:
  1. Discovery & mapping (audit current DNS/hosting, map desired funnels & paths).
  2. DNS & domain connection in GoHighLevel (with a zero-downtime plan if the domain is live).
  3. Funnel routing configuration (mapping each path to the correct funnel or funnel step).
  4. QA, verification & handover.
- Call out specific GoHighLevel concepts:
  - Relationship between Domains, Funnels, Funnel Steps, and Websites.
  - How GHL handles root path vs nested paths.
  - Best practices to avoid one funnel “stealing” the root or catching all paths.
- Mention that you will deliver:
  - A clear path map (`09_ghl_routing_matrix.md`).
  - A DNS/SSL reference (`10_dns_ssl_plan.md`) the client can reuse for future domains.

### Milestones Plan

Suggest a fixed-price milestone breakdown such as:

1. **Phase 1 – Audit & Path Map**
   - Deliverables: documented current DNS state, confirmed desired domain, draft routing matrix.
2. **Phase 2 – DNS + Domain Connection**
   - Deliverables: domain added + verified in GoHighLevel, DNS records configured, SSL active or in progress.
3. **Phase 3 – Funnel Routing & Paths**
   - Deliverables: all agreed paths mapped to correct funnels/steps, internal test links.
4. **Phase 4 – Full QA & Handover**
   - Deliverables: final routing tests, loom walkthrough, updated docs.

Use reasonable hour estimates so this doesn’t look like a $10 task.

### Implementation Checklist

Ensure the checklist explicitly includes:

- Gaining access to:
  - domain registrar or DNS host
  - GoHighLevel account (and correct sub-account, if applicable).
- Capturing the **current** DNS configuration (before changes).
- Configuring DNS records for either:
  - Root domain with ALIAS/ANAME (if supported) or
  - `www` CNAME plus redirects, or
  - Subdomain (e.g. `funnels.domain.com`) pointing to GHL.
- Adding & verifying domain in GHL, attaching it to the correct site/funnel container.
- Setting paths for each funnel and confirming:
  - no duplicated path slugs
  - no “catch-all” conflicts.
- Running routing tests on:
  - desktop + mobile
  - incognito / logged-out sessions
  - with and without trailing slashes.

### Questions for Client

Prioritise questions around:

- Current domain state:
  - Is the domain already live somewhere? If yes, where and can we afford any downtime?
  - Who controls DNS (registrar, Cloudflare, cPanel, etc.)?
- GHL account details:
  - Main account vs sub-account structure.
  - Whether any funnels are already partially mapped to domains.
- Path plan:
  - Exact list of funnels + desired URLs (e.g. `/events`, `/apply`, `/training`, etc.).
  - Preferred behaviour for `/` (root) and `/404`.
- Constraints:
  - Any dates where changes are risky (campaigns running, launches, etc.).
  - Preferred timezone for making DNS changes.

### Proposal Draft

In `06_proposal_draft.md`:

- Open by mirroring the client’s language:
  - Stress that this is **more than just adding a domain**, it’s about clean routing and future-proof structure.
- Make it clear you’ve done **GHL + DNS + multi-funnel path setups** before (phrase in general terms).
- Briefly call out your approach in 3–4 bullets, mapped to the four phases above.
- Address the $10 budget diplomatically by:
  - focusing on value and risk-reduction,
  - implying that the actual scope typically takes more focused expert time than a “quick fix”.
  - It’s fine if you suggest a higher all-in price or a range based on milestones.
- Close with 2–3 sharp questions that show you’ve thought about DNS, routing conflicts, and sub-accounts.

### Risks & Assumptions

Make sure `07_risks_and_assumptions.md` covers at least:

- DNS propagation delays and registrar quirks.
- Incomplete access (no DNS or GHL access granted).
- Existing sites or funnels already tied to the domain.
- Misalignment between the “20 funnels” requested and the actual list the client can provide.
- The fact that configuration can be done quickly, but safe rollout and testing still require a bit of time.

---

After applying all of the above customisations, run the **full standard workflow from the Universal Header** for this job.
