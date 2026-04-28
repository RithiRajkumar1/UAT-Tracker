# UAT Test Cases
## Project: Financial Planning Dashboard | Round 1 | April 2025

---

## Summary

| Total | Passed | Failed | Blocked | Not Run | Pass Rate |
|-------|--------|--------|---------|---------|-----------|
| 20 | 15 | 3 | 1 | 1 | 75% |

---

## Module 1: Dashboard Access

| TC ID | Test Case | Expected Result | Status |
|-------|-----------|----------------|--------|
| TC-001 | Dashboard loads within 5 seconds | Loads in under 5 seconds | ✅ Pass |
| TC-002 | Finance Manager sees all departments | All 4 departments visible | ✅ Pass |
| TC-003 | Dept Head sees only own department | Only own dept shown | ✅ Pass |
| TC-004 | Unauthorised user cannot access | Access denied message shown | ✅ Pass |

---

## Module 2: Budget vs Actuals

| TC ID | Test Case | Expected Result | Status |
|-------|-----------|----------------|--------|
| TC-005 | Correct total budget displayed | Matches approved budget | ✅ Pass |
| TC-006 | Correct total actuals displayed | Matches ERP actuals | ✅ Pass |
| TC-007 | Variance % calculated correctly | Shows percentage format | ❌ Fail |
| TC-008 | Over-budget departments flagged | Warning flag visible | ❌ Fail |
| TC-009 | Department filter works | Only selected dept shown | ✅ Pass |

---

## Module 3: Time Period Filtering

| TC ID | Test Case | Expected Result | Status |
|-------|-----------|----------------|--------|
| TC-010 | Monthly filter shows correct data | Correct month data shown | ✅ Pass |
| TC-011 | Quarterly filter aggregates correctly | 3 months summed correctly | ✅ Pass |
| TC-012 | YTD filter shows cumulative totals | All months from Jan summed | 🔵 Blocked |
| TC-013 | Custom date range works | Selected range data shown | ✅ Pass |

---

## Module 4: Trend Chart

| TC ID | Test Case | Expected Result | Status |
|-------|-----------|----------------|--------|
| TC-014 | Chart displays all 12 months | All months plotted | ✅ Pass |
| TC-015 | Hover tooltip shows data | Month, budget, actual shown | ✅ Pass |
| TC-016 | Chart updates on filter change | Chart updates dynamically | ❌ Fail |

---

## Module 5: Forecast

| TC ID | Test Case | Expected Result | Status |
|-------|-----------|----------------|--------|
| TC-017 | Rolling 3-month forecast correct | AVG of last 3 months shown | ✅ Pass |
| TC-018 | Forecast shown as projected line | Dashed line visible on chart | ✅ Pass |

---

## Module 6: Export

| TC ID | Test Case | Expected Result | Status |
|-------|-----------|----------------|--------|
| TC-019 | Export to Excel works | xlsx file downloaded correctly | ⬜ Not Run |
| TC-020 | Export to PDF works | PDF generated correctly | ✅ Pass |
