# Defect Log
## Project: Financial Planning Dashboard | April 2025

---

## Summary

| Severity | Open | Fixed | Closed |
|----------|------|-------|--------|
| 🔴 Critical | 0 | 0 | 0 |
| 🟠 High | 2 | 0 | 0 |
| 🟡 Medium | 1 | 0 | 0 |
| **Total** | **3** | **0** | **0** |

---

## Defect Register

| DEF ID | Title | Severity | Expected | Actual | Status |
|--------|-------|----------|----------|--------|--------|
| DEF-001 | Variance % showing absolute value | 🟠 High | Shows -4.4% | Shows -£2,200 | 🔴 Open |
| DEF-002 | Over-budget flag not triggering | 🟠 High | Warning flag shown | Status column blank | 🔴 Open |
| DEF-003 | Trend chart not updating on filter | 🟡 Medium | Chart shows filtered dept | Chart shows all depts | 🔴 Open |

---

## DEF-001 Detail

**Severity:** High | **Module:** Budget vs Actuals
**Description:** Variance % column shows currency value instead of percentage, contradicting BR-02.
**Steps to Reproduce:**
1. Login as Finance Manager
2. Navigate to Financial Dashboard
3. Check Variance % column in Department Detail Table

**Expected:** -4.40% in percentage format
**Actual:** -£2,200 in currency format
**Business Impact:** Finance team cannot compare proportional variance across departments of different budget sizes.
**Fix Required:** Apply formula (actual-budget)/budget x 100 and format as percentage.

---

## DEF-002 Detail

**Severity:** High | **Module:** Budget vs Actuals
**Description:** Over-budget warning flag not appearing for Operations dept despite 13.7% overspend, contradicting BR-06.
**Steps to Reproduce:**
1. Login as Finance Manager
2. Navigate to Financial Dashboard
3. View Operations department row
4. Check Status column

**Expected:** OVER BUDGET warning flag
**Actual:** Status column is blank
**Business Impact:** CFO cannot identify overspending departments without manual calculation.
**Fix Required:** If variance % is less than -10 then display OVER BUDGET flag.

---

## DEF-003 Detail

**Severity:** Medium | **Module:** Trend Chart
**Description:** Trend chart does not respond to department filter changes while other components update correctly.
**Steps to Reproduce:**
1. Login as Finance Manager
2. Navigate to Financial Dashboard
3. Select Finance from Department dropdown
4. Observe Trend Chart

**Expected:** Chart shows only Finance department data
**Actual:** Chart still shows all departments
**Workaround:** Use individual department report page until fix is deployed.
**Fix Required:** Trend chart must subscribe to same filter context as rest of dashboard.
