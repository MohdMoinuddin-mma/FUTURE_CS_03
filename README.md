# FUTURE_CS_03 — API Security Risk Analysis

**Future Interns Cyber Security Internship Program 2026**
**Intern:** Mohammad Moinuddin
**CIN ID:** FIT/FEB26/CS6460
**Track:** Cyber Security (CS)
**Task:** Task 3 — API Security Risk Analysis

---

## 📌 Overview

This repository contains the API Security Risk Analysis Report conducted on **JSONPlaceholder** — a public REST API used for testing and prototyping. The assessment was performed ethically using read-only GET requests only, following the OWASP API Security Top 10 (2023) framework.

---

## 🎯 API Tested

| Detail | Info |
|---|---|
| API Name | JSONPlaceholder |
| Base URL | https://jsonplaceholder.typicode.com |
| API Type | Public REST API (demo/test environment) |
| Auth Required | None (finding in itself) |

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Postman v11 | API request testing & response inspection |
| Browser DevTools | Header analysis |
| OWASP API Security Top 10 | Assessment framework |

---

## 🔍 Endpoints Tested

- `GET /users` — All user records
- `GET /users/1` — Single user by ID (IDOR test)
- `GET /users/999` — Invalid ID (error handling test)
- `GET /comments` — Comments with PII exposure test
- `GET /posts` — Pagination test

---

## 🚨 Findings Summary

| # | Finding | Severity |
|---|---|---|
| 1 | No Authentication on Endpoints | HIGH |
| 2 | Insecure Direct Object Reference (IDOR) | HIGH |
| 3 | Excessive Data Exposure in /comments | HIGH |
| 4 | Missing Critical Security Headers | MEDIUM |
| 5 | No Pagination — Mass Data Dump | MEDIUM |
| 6 | Technology Stack Disclosure | LOW |

---

## 📁 Repository Structure
```
FUTURE_CS_03/
├── README.md
├── report/
│   └── API_Security_Risk_Analysis_Report.pdf
└── evidence/
    ├── 01_users_response.png
    ├── 02_headers_part1.png
    ├── 03_headers_part2.png
    ├── 04_users_by_id.png
    ├── 05_users_999_404.png
    ├── 06_comments_response.png
    └── 07_posts_response.png
```

---

## ⚠️ Ethical Statement

All testing was conducted using read-only GET requests only. No exploitation, authentication bypass, brute force, or denial-of-service testing was performed. JSONPlaceholder is a public demo API built specifically for safe testing.

---

## 🔗 References

- [OWASP API Security Top 10](https://owasp.org/API-Security/)
- [JSONPlaceholder](https://jsonplaceholder.typicode.com)
- [Future Interns](https://www.linkedin.com/company/future-interns)
```
