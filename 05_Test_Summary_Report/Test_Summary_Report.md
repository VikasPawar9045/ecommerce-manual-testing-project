# Test Summary Report — E-Commerce Website

**Version:** 1.0 | **Prepared By:** Vikas | **Date:** 05-Jul-2026 | **Cycle:** 1

---

## 1. Purpose

This report summarizes the manual testing activities, results, and defects identified during Test Cycle 1 for the E-Commerce Website project, along with a release recommendation.

## 2. Test Execution Overview

| Metric | Value |
|---|---|
| Total Test Cases Planned | 52 |
| Total Test Cases Executed | 52 (100%) |
| Passed | 46 (88.5%) |
| Failed | 6 (11.5%) |
| Blocked / Not Executed | 0 |
| Total Requirements | 18 |
| Requirement Coverage | 18/18 (100%) |
| Total Defects Logged | 6 |

## 3. Module-Wise Execution Summary

| Module | Test Cases | Pass | Fail |
|---|---|---|---|
| User Registration | 7 | 6 | 1 |
| User Login | 7 | 6 | 1 |
| Product Search & Filter | 7 | 6 | 1 |
| Shopping Cart | 8 | 7 | 1 |
| Checkout & Payment | 10 | 8 | 2 |
| Order Management | 5 | 5 | 0 |
| Wishlist | 4 | 4 | 0 |
| User Profile | 4 | 4 | 0 |
| **Total** | **52** | **46** | **6** |

## 4. Defect Summary by Severity

| Severity | Count | Bug IDs |
|---|---|---|
| Critical | 2 | BUG_002, BUG_006 |
| Major | 4 | BUG_001, BUG_003, BUG_004, BUG_005 |
| Minor | 0 | — |

## 5. Defect Summary by Status

| Status | Count |
|---|---|
| Open | 5 |
| In Progress | 1 |
| Fixed | 0 |
| Closed | 0 |

## 6. Key Observations

- **Checkout & Payment** module has the highest concentration of defects (2 of 10 test cases failed), including one **Critical** severity issue (duplicate order on double-click) — this module needs priority attention before release.
- **Login security** gap identified: no account lockout mechanism after repeated failed attempts (BUG_002), which is a **Critical** security-adjacent risk.
- **Order Management, Wishlist, and User Profile** modules passed 100% of executed test cases and are considered stable.
- All 18 mapped requirements have at least one executed test case — full functional coverage achieved for this cycle.

## 7. Recommendation

🔴 **Not recommended for production release** in current state due to 2 open Critical defects (BUG_002, BUG_006) impacting login security and payment integrity.

**Suggested next steps:**
1. Fix and retest BUG_002 (account lockout) and BUG_006 (duplicate order on double payment click) — both Critical.
2. Fix and retest the 4 Major defects, prioritizing BUG_005 (tax calculation) as it directly affects order amounts.
3. Conduct a focused **Retest cycle (Cycle 2)** on Checkout & Payment and Login modules only.
4. Re-evaluate release readiness after Cycle 2 sign-off.

## 8. Sign-off

| Role | Name | Status |
|---|---|---|
| QA Tester | Vikas | Testing Complete — Cycle 1 |
| Product Owner | — | Pending Review |
