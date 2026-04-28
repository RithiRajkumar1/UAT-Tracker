# 🧪 UAT Tracking & Defect Management Framework

A reusable User Acceptance Testing framework for Business Analysts covering test planning, test case documentation, defect logging, and go-live readiness tracking.

## 📋 UAT Lifecycle

1. UAT PLANNING — Define scope, entry and exit criteria, timeline
2. TEST CASE PREPARATION — Write test cases mapped to requirements
3. TEST EXECUTION — Execute cases, log pass, fail or blocked
4. DEFECT MANAGEMENT — Log defects, assign severity, track resolution
5. REGRESSION TESTING — Re-test fixed defects
6. SIGN-OFF — Stakeholder approval for go-live

## 🚦 Defect Severity Guide

| Severity | Definition | SLA |
|----------|-----------|-----|
| 🔴 Critical | System crash, data loss | Fix before UAT continues |
| 🟠 High | Major feature broken, no workaround | Fix within 24 hours |
| 🟡 Medium | Feature partially working, workaround exists | Fix before go-live |
| 🟢 Low | Minor UI or cosmetic issue | Fix in next release |

## ✅ Entry Criteria — Before UAT Begins

- All functional requirements signed off
- UAT environment deployed and stable
- Test data prepared and loaded
- Test cases reviewed and approved
- UAT participants identified and available

## ✅ Exit Criteria — Before Go-Live

- 100% of test cases executed
- 0 Critical defects open
- 0 High defects open
- All Medium defects have approved workarounds
- Stakeholder sign-off obtained

## 📁 Files in this Repo

| File | Description |
|------|-------------|
| Test_Cases_Financial_Dashboard.md | 20 test cases with pass and fail status |
| Defect_Log.md | Defect tracking register with detailed defect cards |
