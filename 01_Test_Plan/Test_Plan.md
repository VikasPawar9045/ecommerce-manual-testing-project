# Test Plan — E-Commerce Website (Online Shopping Platform)

**Version:** 1.0 | **Prepared By:** Vikas | **Date:** 02-Jul-2026

---

## 1. Introduction

This document defines the test strategy, scope, approach, resources, and schedule for manual testing of the E-Commerce Website. The application allows users to register/login, search and browse products, manage a shopping cart, complete checkout with multiple payment options, and manage their orders, wishlist, and profile.

## 2. Objectives

- Ensure all core e-commerce workflows function correctly end-to-end
- Validate both positive and negative scenarios for each module
- Identify and log defects before release to production
- Ensure 100% requirement coverage through traceability
- Provide stakeholders with a clear go/no-go recommendation via test summary reporting

## 3. Scope

### 3.1 In Scope
- User Registration & Login (including password reset, account lockout)
- Product Search, Filtering & Sorting
- Shopping Cart (add/update/remove, coupons, stock validation)
- Checkout Process (address management, order summary)
- Payment Gateway (Card, UPI, Cash on Delivery)
- Order Management (history, tracking, cancellation, invoice)
- Wishlist functionality
- User Profile & Account Settings
- Functional, UI, and negative/boundary testing (manual, black-box)

### 3.2 Out of Scope
- Performance / Load testing
- Security / Penetration testing (beyond basic negative-path validation)
- Automated regression testing
- Mobile app testing (iOS/Android native apps)
- Third-party payment gateway internal testing (only integration touchpoints tested)
- Localization / multi-language testing

## 4. Test Approach / Strategy

Testing will be conducted manually using **Black-Box Testing** techniques:

| Technique | Applied To |
|---|---|
| Equivalence Partitioning | Search inputs, price filters, form fields |
| Boundary Value Analysis | Cart quantity limits, stock thresholds, password length |
| Positive Testing | Verifying core happy-path workflows |
| Negative Testing | Invalid inputs, edge cases, error handling |
| Exploratory Testing | Ad-hoc checks around checkout & payment flows |

**Test Levels:** System Testing (end-to-end functional flows), with focus on integration between modules (e.g., Cart → Checkout → Payment → Order).

## 5. Test Environment

| Component | Details |
|---|---|
| Application Type | Web-based E-commerce Platform |
| Browsers | Chrome (latest), Firefox (latest), Edge |
| OS | Windows 11 |
| Test Data | Dummy user accounts, test card numbers (sandbox), test coupon codes |
| Test Management | Excel-based (Test Cases, Bug Reports, RTM) |

## 6. Entry Criteria

- Test cases reviewed and approved
- Build/environment deployed and accessible for testing
- Test data prepared (user accounts, product catalog, coupons)
- Requirements/user stories finalized

## 7. Exit Criteria

- 100% of planned test cases executed
- No open **Critical** severity defects
- All **High priority** defects triaged (Fixed or accepted with sign-off)
- Test Summary Report shared with stakeholders

## 8. Test Deliverables

- Test Plan (this document)
- Test Cases (`Test_Cases_Ecommerce.xlsx`)
- Bug/Defect Reports (`Bug_Reports.xlsx`)
- Requirement Traceability Matrix (`Traceability_Matrix.xlsx`)
- Test Summary Report

## 9. Roles & Responsibilities

| Role | Responsibility |
|---|---|
| QA Tester (Vikas) | Test case design, execution, defect logging, reporting |
| Developer | Defect fixes, root cause clarification |
| Product Owner | Requirement clarification, UAT sign-off |

## 10. Risk & Mitigation

| Risk | Impact | Mitigation |
|---|---|---|
| Ambiguous/changing requirements | Test case rework | Maintain close communication with Product Owner; version test cases |
| Limited test environment stability | Delayed execution | Schedule execution in stable environment windows; log environment-specific issues separately |
| Payment gateway sandbox limitations | Cannot test all real-world payment scenarios | Use documented sandbox test cards/UPI IDs; note as an assumption |
| Time constraints | Reduced test coverage | Prioritize test cases by risk (Critical/High modules first — Checkout & Payment) |

## 11. Test Schedule (Sample)

| Phase | Duration |
|---|---|
| Test Planning & Test Case Design | Day 1–2 |
| Test Case Review | Day 3 |
| Test Execution (Cycle 1) | Day 4–6 |
| Defect Retesting & Regression | Day 7 |
| Test Summary Reporting | Day 8 |

## 12. Assumptions

- Test environment mirrors production configuration closely enough for functional validation
- Sandbox payment credentials are available and behave consistently
- Test data (users, products, coupons) is pre-seeded and does not require creation from scratch during execution
