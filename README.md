# Cyber Law & Ethics Analysis — Techfite Case

A legal and ethical analysis of a corporate insider-misuse scenario, identifying which U.S.
federal computer-crime statutes were violated, evaluating the conduct against professional
ethical frameworks, and mapping the failures to compliance controls that would have prevented
them.

> Scenario-based lab. "Techfite" and all individuals are fictional.

## Scenario

At Techfite, monitoring logs showed that dummy accounts (created at the request of a manager,
Carl Jaspers) were used to access financial and executive documents without authorization,
and that penetration tools (Metasploit) and network scanning were run against other business
units without approval.

## Part 1 — Legal analysis

| Conduct | Statute violated | Why |
|---|---|---|
| Dummy accounts accessing financial/executive docs without authorization | **CFAA** (18 U.S.C. § 1030) | Unauthorized access to a protected computer / exceeding authorized access |
| Running Metasploit and scanning other units' networks without approval | **ECPA** (18 U.S.C. § 2510 et seq.) | Unauthorized interception/access of electronic communications |

The analysis walks through the elements of each statute and ties specific log evidence to
each element, then discusses potential criminal and civil exposure for the individuals and
the company.

## Part 2 — Ethics analysis

Evaluated against professional codes (e.g., the ISSA code of ethics — "perform all
professional activities and duties in accordance with all applicable laws and the highest
ethical principles"). Had Techfite adopted and enforced such guidelines, the creation and use
of dummy accounts would have been discouraged and flagged. The analysis contrasts the
individual actors' choices with the duties of confidentiality, integrity, and lawful conduct,
and identifies where management failed its ethical obligations.

## Part 3 — Compliance mapping

The core failure was a governance gap: no separation of duties, no access review, no logging
follow-through. [`compliance-mapping.csv`](./compliance-mapping.csv) maps each failure to the
control that would have caught or prevented it (NIST SP 800-53, SOX where financial data is
involved, and general least-privilege/audit principles).

## What's in this repo

- `README.md` — this case study.
- `compliance-mapping.csv` — failure → violated law/standard → preventive control.
- `legal-frameworks-reference.md` — plain-language summaries of CFAA, ECPA, SOX, and GDPR
  relevance for security practitioners.

## Skills demonstrated

Applying CFAA/ECPA to real conduct · evidence-to-element legal reasoning · professional ethics
frameworks · governance & separation-of-duties analysis · compliance control mapping (NIST
800-53 / SOX).
