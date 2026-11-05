# Statement of Work — Template

**Engagement:** [Service name]
**Client:** [Legal entity name + country]
**Contractor:** Abd Alrahaman Mohamed (GitHub @61465)
**Effective date:** [YYYY-MM-DD]
**SOW version:** 1.0

---

## 1. Scope

**1.1 Deliverables**
- [Specific artifact 1, e.g. "written security audit report (PDF + markdown)"]
- [Specific artifact 2, e.g. "up to 3 pull requests against client repository"]
- [Specific artifact 3, e.g. "60-minute debrief call with client engineering lead"]

**1.2 Out of scope**
- Changes to any system Contractor has not been granted explicit access to
- Any work outside the subject repository/service
- Testimonials or public attribution without written consent of both parties

**1.3 Assumptions**
- Client provides read access to the subject codebase on day 1
- Client designates a single point-of-contact for questions
- Client responds to blocker-questions within one business day

---

## 2. Timeline

- **Kickoff:** [Date]
- **Mid-engagement check-in:** [Date]
- **Deliverable due:** [Date]
- **Revision window ends:** [Date + 10 business days]

Total engagement duration: [N] business days.

---

## 3. Fees

- **Fixed fee:** USD [amount], inclusive of all Contractor expenses
- **OR Hourly rate:** USD [rate]/hour, invoiced in 30-minute increments, capped at [N] hours without pre-approval

**Payment terms**
- Fixed-price: 50% upon SOW execution, 50% upon deliverable acceptance
- Hourly: net-15 from monthly invoice
- Currency: USD only
- Method: Wise, Payoneer, or direct USD bank transfer

**Late payment:** 1.5% per month on balance >15 days past due.

---

## 4. Intellectual property

- Contractor assigns all deliverable IP to Client upon full payment
- Methodology, tooling, and scanner source code developed prior to engagement remain Contractor's property
- Contractor may reference the engagement (client name + high-level scope) in public portfolio **only with Client's written consent** per Section 7

---

## 5. Confidentiality

- All Client data, source code, and findings are confidential
- Contractor will not disclose findings to third parties, including vendors of Client's dependencies, without Client's written consent
- Exception: if Contractor discovers a vulnerability in a third-party library that affects multiple parties, Contractor will coordinate responsible disclosure with Client's approval
- Confidentiality survives termination for 3 years

---

## 6. Responsible-disclosure clause

If this engagement surfaces a security vulnerability in a third-party dependency:

- Contractor will **not** file a security advisory under Contractor's name without Client's written consent
- Contractor will **not** collect bug bounties for findings discovered during this engagement
- Client has first right of coordinated disclosure
- If Client declines to disclose within 30 days, parties negotiate joint disclosure or Contractor withdrawal

This clause protects both parties from unexpected media exposure.

---

## 7. Public attribution

- **Default:** no public attribution. Engagement is private.
- **Opt-in:** Client may consent in writing to Contractor listing engagement on public portfolio (e.g., "Audited identity integration for [Client] in Nov 2026")
- **Testimonial:** Client may provide a written testimonial. Contractor may quote with Client's approval of exact wording.

---

## 8. Termination

- Either party may terminate with 48-hour written notice
- Upon termination: Contractor invoices for work completed through termination date; Client pays within net-15
- No cancellation penalties beyond the 50% retainer for fixed-price engagements

---

## 9. Warranties & liability

- Contractor warrants work is performed with reasonable skill and care
- Contractor does NOT warrant discovery of all vulnerabilities, bugs, or performance issues
- Liability cap: equal to total fees paid under this SOW
- No consequential, indirect, or punitive damages

---

## 10. Governing law

- English law unless mutually agreed otherwise in writing
- Any dispute first addressed via 30 days good-faith negotiation
- Then LCIA arbitration, seat London, one arbitrator

---

## 11. Signatures

**For Client:**
Name: _______________________________
Title: _______________________________
Signature: _______________________________
Date: _______________________________

**For Contractor:**
Name: Abd Alrahaman Mohamed
Title: Independent Contractor
Signature: _______________________________
Date: _______________________________

---

## Appendix A — Deliverable acceptance criteria

[List specific objective criteria for accepting each deliverable, e.g.:]

- Written report: delivered as PDF + markdown, minimum 10 pages, covers all in-scope areas
- Pull requests: pass client's CI suite, do not touch out-of-scope code, each PR independently reviewable
- Debrief call: scheduled within 5 business days of report delivery

---

## Appendix B — Access requirements

[List what the Contractor needs from the Client to start work, e.g.:]

- Read-only access to repository [name]
- VPN credentials: [yes/no]
- Access to test environment: [yes/no]
- Point-of-contact email: [name@client.com]
