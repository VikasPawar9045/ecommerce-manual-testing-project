# 🛒 E-Commerce Website — Manual Testing Portfolio Project

A complete, real-world style **Manual QA Testing project** built on a sample E-commerce web application (product search, cart, checkout & payment). This repository demonstrates end-to-end manual testing skills — from test planning to execution, defect reporting, and requirement traceability — following industry-standard STLC practices.

## 📌 Project Overview

| | |
|---|---|
| **Application Under Test (AUT)** | Online Shopping Platform (Web) |
| **Testing Type** | Manual Functional Testing |
| **Modules Covered** | Registration, Login, Search & Filter, Cart, Checkout & Payment, Order Management, Wishlist, Profile |
| **Total Test Cases** | 52 |
| **Total Requirements Mapped** | 18 |
| **Defects Logged** | 6 |
| **Tools Used** | Excel, Manual STLC documentation, GitHub |

## 🎯 Objective

This project simulates a real QA assignment where a tester is given a new e-commerce feature set and is responsible for:
1. Writing a formal **Test Plan**
2. Designing detailed **Test Cases** covering positive, negative, and boundary scenarios
3. **Executing** test cases and logging results
4. Raising and tracking **Bug Reports** for failures found
5. Maintaining a **Requirement Traceability Matrix (RTM)** to ensure full coverage
6. Summarizing results in a **Test Summary Report**

## 📁 Repository Structure

```
ecommerce-manual-testing-project/
│
├── 01_Test_Plan/
│   └── Test_Plan.md                    → Scope, approach, entry/exit criteria, schedule
│
├── 02_Test_Cases/
│   └── Test_Cases_Ecommerce.xlsx       → 52 detailed test cases across 8 modules
│
├── 03_Bug_Reports/
│   └── Bug_Reports.xlsx                → 6 defects logged from failed test cases
│
├── 04_Traceability_Matrix/
│   └── Traceability_Matrix.xlsx        → 18 requirements mapped to test cases
│
├── 05_Test_Summary_Report/
│   └── Test_Summary_Report.md          → Execution summary, metrics & recommendations
│
└── README.md
```

## 🧩 Modules Tested

- **User Registration** — field validation, duplicate email, password policy
- **User Login** — valid/invalid login, account lockout, forgot password
- **Product Search & Filter** — keyword search, filters, sorting, edge cases
- **Shopping Cart** — add/update/remove items, coupon codes, stock validation
- **Checkout & Payment** — address selection, Card/UPI/COD, payment failure handling
- **Order Management** — order history, tracking, cancellation, invoice download
- **Wishlist** — add/remove/move-to-cart, guest user flow
- **User Profile** — profile update, password change, address book

## 🐞 Sample Defects Found

| Bug ID | Title | Severity |
|---|---|---|
| BUG_002 | No account lockout after repeated failed login attempts | Critical |
| BUG_006 | Duplicate order created on rapid double-click of Pay Now | Critical |
| BUG_001 | Weak password accepted despite validation warning | Major |
| BUG_004 | Cart quantity not capped to available stock | Major |
| BUG_005 | Incorrect tax calculation on order summary | Major |
| BUG_003 | Blank white screen on search with special characters | Major |

*(Full details with steps to reproduce in `03_Bug_Reports/Bug_Reports.xlsx`)*

## 📊 Test Execution Summary

- **Total Test Cases:** 52
- **Passed:** 46 (88.5%)
- **Failed:** 6 (11.5%)
- **Requirement Coverage:** 18/18 (100%)

Full breakdown available in `05_Test_Summary_Report/Test_Summary_Report.md`.

## 🛠️ Skills Demonstrated

- Test Plan creation (Scope, Approach, Entry/Exit Criteria)
- Test Case design techniques (Equivalence Partitioning, Boundary Value Analysis, Positive/Negative testing)
- Manual test execution & result logging
- Defect Life Cycle / Bug reporting with severity & priority classification
- Requirement Traceability Matrix (RTM) for coverage tracking
- Test Summary Reporting

## 👤 Author

**Vikas**
Data Analyst | Aspiring SDET
📍 Noida, India

---
*This is a self-initiated portfolio project created to demonstrate manual QA testing skills for Data Analyst / SDET job applications. The application under test is a hypothetical e-commerce platform used for demonstration purposes only.*
