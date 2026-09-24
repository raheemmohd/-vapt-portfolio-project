# Web Application Security Testing Lab — Recon to Remediation

An interactive walkthrough of an authorized web application penetration test — from reconnaissance and enumeration through confirmed findings, risk scoring, and a client-ready report. Built as a single self-contained web page, no backend or build step required.

**[▶ Live demo](https://raheemmohd.github.io/vapt-portfolio-project/)**

![status](https://img.shields.io/badge/status-complete-brightgreen) ![type](https://img.shields.io/badge/type-portfolio%20project-blue) ![stack](https://img.shields.io/badge/stack-HTML%2FCSS%2FJS-informational)

---

## Why I built this

I wanted to show VAPT methodology the same way I documented my SOC project — something a reviewer can click through, not just read about. This page walks through the full five-phase testing methodology (recon → scanning → vulnerability analysis → exploitation → reporting), with two fully worked case studies: a SQL injection in a login form, and a broken access control (IDOR) flaw in an API. Both include the actual request/response evidence, OWASP mapping, and a CVSS-style risk score, then end with a live findings queue you can triage yourself.

## What's inside

| Section | What it covers |
|---|---|
| Testing methodology | The 5-phase PTES/OWASP approach, plus scope and black/gray/white box testing |
| Reconnaissance flowchart | Passive recon → subdomain enumeration → live host confirmation → active scanning decision |
| Tools & sample commands | Nmap scan commands and sample output, the Burp Suite workflow, a tool-category reference table |
| OWASP Top 10 reference | Quick-reference table of the categories every test is checked against |
| Risk scoring model | A CVSS-style formula (exploitability × impact × data sensitivity) with a worked table |
| Case study 1 | SQL injection in a login form — discovery, validation, scope-limited impact demo, remediation |
| Case study 2 | IDOR in an invoices API — discovery, validation, impact, remediation |
| Reporting | What every finding needs, and the executive-summary vs. technical-detail split |
| **Live demo — findings queue** | 5 findings of varying severity; view evidence, then classify each one |
| Metrics that matter | Time to remediate, re-test pass rate, OWASP coverage, severity mix |
| Where VAPT is heading | Continuous pentesting, AI-assisted discovery, attack surface management, shift-left security |

## Skills demonstrated

`Reconnaissance & OSINT` · `Nmap scanning & enumeration` · `Burp Suite (Proxy/Repeater/Intruder)` · `Manual vulnerability testing` · `SQL injection` · `Broken access control / IDOR` · `OWASP Top 10` · `CVSS-style risk scoring` · `Vulnerability report writing`

## Tech stack & approach

Pure HTML, CSS, and vanilla JavaScript — no frameworks, no dependencies, no build tooling. All diagrams are hand-built inline SVG rather than screenshots, and the findings queue is a small state machine in plain JS. Same reasoning as my SOC project: dependency-free means anyone can host it or read the whole source in one sitting.

## Running it locally

```bash
git clone https://github.com/raheemmohd/vapt-portfolio-project.git
cd vapt-portfolio-project
open index.html
```

## A note on the data

All targets, requests, responses, hostnames, and findings shown are synthetic, built to illustrate a realistic testing workflow — no real system, client, or organization is represented. Every technique described here is only legal and ethical when performed against systems you have explicit written authorization to test.

## License

MIT

## Author

Mohammed Abdul Raheem
