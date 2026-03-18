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

---

## 🚀 Step-by-Step GitHub Upload

**Step 1 — Create a GitHub account** (skip if you have one)
Go to github.com → Sign up → verify your email

---

**Step 2 — Create the repository**
1. Click the **+** button (top right) → **New repository**
2. Repository name: `FUTURE_CS_03`
3. Set it to **Public** ✅ (required by Future Interns)
4. Check **"Add a README file"** ✅
5. Click **Create repository**

---

**Step 3 — Edit the README**
1. You'll see `README.md` in your repo — click the **pencil icon** ✏️ to edit
2. Select all the existing text → delete it
3. Paste the README content from above
4. Scroll down → click **Commit changes** → **Commit changes** again

---

**Step 4 — Upload your PDF report**
1. In your repo, click **Add file** → **Upload files**
2. Create a folder path by typing `report/` before the filename — GitHub will auto-create the folder
3. Drag and drop your `API_Security_Risk_Analysis_Report.pdf`
4. Scroll down → click **Commit changes**

---

**Step 5 — Upload your screenshots**
1. Click **Add file** → **Upload files** again
2. Upload all 7 Postman screenshots
3. Name them clearly:
   - `01_users_response.png`
   - `02_headers_part1.png`
   - `03_headers_part2.png`
   - `04_users_by_id.png`
   - `05_users_999_404.png`
   - `06_comments_response.png`
   - `07_posts_response.png`
4. Click **Commit changes**

---

**Step 6 — Verify your repo looks like this:**
```
FUTURE_CS_03/
├── README.md          ✅
├── report/
│   └── ...pdf         ✅
└── evidence/
    └── ...screenshots ✅
```

---

**Step 7 — Copy your repo link**
Your repo URL will be:
```
https://github.com/YOUR_USERNAME/FUTURE_CS_03
