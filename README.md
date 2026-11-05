# @61465 / services

**Public pricing and engagement terms for short-term consulting.**

Maintained as a separate repo so pricing is versioned and discoverable via GitHub search. Last updated: 2026-11-05.

---

## 1. Identity Integration Audit

**Problem:** Your auth/SSO integration might have a Provider Trust Boundary (PTB) bug — the class behind Microsoft nOAuth, GitHub `verified`-bypass, and four accepted GHSAs in the last 30 days against Supabase, Hanko, Documenso, Auth.js.

**What you get:**
- 5 business-day engagement
- End-to-end review of the IdP handshake, token validation, account linking, signup recovery paths
- Written report (PDF + markdown) with CVSS-scored findings
- Up to 3 pull requests with proposed fixes (ready to merge, your call)
- One 60-minute debrief call

**Fit:** You added "Sign in with X" in the last 12 months. You use `@auth/*`, `better-auth`, Supabase Auth, Hanko, Clerk, Casdoor, Keycloak, or you rolled your own. You've never had an external security review of the integration.

**Price:** $1,990 flat (startup / pre-Series-A) · $5,000 flat (enterprise)

**Proof:**
- [github.com/61465/ptb-report-card](https://github.com/61465/ptb-report-card) — the methodology, public, MIT-licensed
- 4 accepted GHSAs in Oct 2026 across 4 vendors, same class
- CWE proposal submitted to MITRE (PTB class) · Node.js security-wg RFC #1593

---

## 2. Crisis Response

**Problem:** A CVE just dropped on one of your dependencies. Your prod is unhappy. Your security team needs a backport by Friday. The OSS maintainer is on vacation.

**What you get:**
- Same-week start (24-hour response)
- Hands-on debugging, patch authoring, upstream coordination
- If upstream is the blocker: I'll open the PR, respond to reviews, chase the merge
- Written daily status update to stakeholders

**Fit:** You need senior OSS judgment and PR-merging credibility on day one. You don't have time for a two-week onboarding.

**Price:** $125/hour (startup) · $200/hour (enterprise). 10-hour minimum. 30-minute increments.

**Proof:** 10+ merged OSS PRs across Sentry, PostHog, Supabase, Ory, Drizzle, Inngest, rrweb. Public ledger on profile.

---

## 3. Performance Hunt

**Problem:** Your app is slow somewhere but you can't find it. You suspect an algorithmic issue but your APM blames the network.

**What you get:**
- 3-day scan for O(n²)/O(n log n) hotspots using a defined methodology
- A working PR with before/after benchmarks for each confirmed finding
- You pay per *confirmed* finding (success-based)

**Fit:** You have a reproducible slow path. You're on TypeScript, Rust, Go, Python, or Node.

**Price:** $1,000 per confirmed find (startup) · $2,500 per confirmed find (enterprise). No finds = no invoice.

**Proof:** PostHog PR #5244 — found an O(n²) in `rrweb.MutationBuffer.processBufferedMutations` that caused 10-second main-thread freezes on 500-row shadow-DOM batches. Fixed, benchmarked, merged, shipped in rrweb next release.

---

## 4. LLM Cost Audit

**Problem:** Your LLM bill is growing faster than your usage. Nobody knows why. Your CFO asks for a plan and you have a hunch, not a number.

**What you get:**
- Measure current cost per request end-to-end: input, output, retries, fallback tier
- HSTC-methodology compression trial on your actual prompts (zero-LLM, deterministic, drop-in)
- Written report with projected savings under 4 scenarios + confidence intervals
- Reference implementation in your language of choice

**Fit:** You're spending >$5K/month on a single LLM provider. You've already tried "cheaper model" and want something more interesting.

**Price:** $2,490 flat (startup) · $7,500 flat (enterprise)

**Proof:**
- [github.com/61465/local-first-langchain-bench](https://github.com/61465/local-first-langchain-bench) — HSTC methodology, 49–57% input-token reduction measured on 3 tokenizers (Groq / Gemini / tiktoken)
- Live Feature Request on `langchain-ai/langchain#41718` with cross-provider validation attached

---

## 5. OSS Rescue PR

**Problem:** Your product is blocked on a bug in an upstream dependency. The maintainer has 400 open issues. You can't ship a fork.

**What you get:**
- I take ownership of the PR end-to-end
- Reproduce, debug, write, test, submit, respond to reviews, chase the merge
- You get either a merged PR or a working private branch + tracking issue

**Fit:** You've already identified the upstream project and bug. You just need someone to push it through.

**Price:** $500 per merged PR (startup) · $1,500 per merged PR (enterprise). Price locked at engagement start. If the PR doesn't merge within 60 days, 50% refund.

**Proof:** 10+ merged PRs. Named maintainers who have approved/merged my work: @vjeranc (Sentry Relay), @marandaneto (PostHog), @ferhatelmas (Supabase), @teemingc (SvelteKit), @eoghanmurray (rrweb).

---

## Not offered

- Full-time employment (ask on LinkedIn: `abdalrahman-gz`)
- Long-term retainers before first engagement closes
- Security-advisory submission as a service (ethical issues; vendors deal with me directly)
- Anything requiring access to your prod secrets without a signed DPA

---

## Terms

- **SOW required** for every engagement, even $500 PRs
- **50% upfront** for fixed-price · **net-15** for hourly
- **Mutual NDA** on request
- **Payment:** Wise, Payoneer, USD bank transfer. No PayPal, no crypto
- **Jurisdiction:** engagements governed by English law unless mutually agreed otherwise
- **Right of refusal:** I decline work that conflicts with ongoing OSS relationships or responsible-disclosure commitments

---

## Contact

`abdarahman10555@gmail.com` — response within 24h on business days.

Email with: your repo/library, the symptom, the timeline. The first reply will either (a) scope + rate confirmation or (b) honest "not a fit, here's who might be."
