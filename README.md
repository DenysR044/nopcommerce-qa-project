# nopCommerce QA Project

Independent manual QA project for the nopCommerce Demo Store.

**Application Under Test:** [nopCommerce Demo Store](https://demo.nopcommerce.com/)

The project demonstrates the complete manual testing process: test planning, user stories, test scenarios, test cases, test execution, bug reporting, exploratory testing, and test summary.

## Project Goal

The goal of this project is to evaluate the main customer flows of the nopCommerce Demo Store and verify that users can successfully search for products, manage the shopping cart, complete checkout, place orders, and manage their account and orders.

## Scope

The following areas were tested:

- Registration and authentication
- Password recovery
- Account management
- Product search
- Product browsing, filtering, and sorting
- Product details
- Shopping cart
- Checkout and payment
- Order placement
- Order history and order management
- Order status

The project focuses on the registered customer flow.

Performance, load, security, mobile application, admin panel, third-party payment gateway internals, and guest checkout testing were outside the project scope.

## Test Types

- Smoke Testing
- Functional Testing
- UI Testing
- Negative Testing
- Exploratory Testing
- End-to-End Testing

## Test Documentation

| Document | Description |
|---|---|
| [Test Plan](1.%20test-plan.md) | Testing scope, objectives, environment, test types, test data, risks, and priorities |
| [User Stories](2.%20user-stories.md) | 14 user stories describing the main customer flows |
| [Test Scenarios](3.%20test-scenarios.md) | 102 test scenarios covering the defined user stories and end-to-end flow |
| [Test Cases](4.%20test-cases.xlsx) | 138 detailed test cases |
| [Test Execution](5.%20test-execution.xlsx) | Smoke and full test execution results |
| [Bug Reports](6.%20bug-reports.md) | 6 documented defects with steps, expected and actual results, and evidence |
| [Exploratory Testing](7.%20exploratory-testing.md) | 4 exploratory testing sessions with findings and observations |
| [Test Summary](8.%20test-summary.md) | Final testing results, defect summary, key findings, and conclusion |

> **Note:** Excel files are not fully previewed directly by GitHub. Download the `.xlsx` files to view the complete spreadsheets.

## Test Results

### Smoke Test

- Total: 10
- Passed: 10
- Failed: 0
- Blocked: 0

### Full Test Execution

- Total: 138
- Passed: 134
- Failed: 1
- Blocked: 3

**Overall Result:** Completed with Issues

## Defects

A total of 6 defects were documented:

- 1 Major
- 5 Minor

Priority distribution:

- 1 High
- 4 Medium
- 1 Low

The main functional issue affected the password recovery flow. The recovery request was accepted, but the recovery email was not received, which blocked three dependent test cases.

Additional defects were found during exploratory testing in validation behavior, catalog data, product search, and product metadata.

Evidence screenshots are stored in the [`screenshots`](screenshots/) folder.

## Exploratory Testing

Four exploratory testing sessions were completed:

- ET-001 - Checkout Address Validation
- ET-002 - Registration and Password Validation
- ET-003 - Search and Product Discovery
- ET-004 - Shopping Cart

Exploratory testing identified additional defects and helped verify behavior that was not fully covered by predefined test cases.

## Key Findings

- The main purchase flow was successfully completed.
- Registration, login, product browsing, shopping cart, checkout, payment, order placement, and order management worked during testing.
- Password recovery could not be fully completed because the recovery email was not received.
- Several validation and catalog data inconsistencies were identified.
- Search by a regular product SKU worked, but search by SKUs assigned to product attribute combinations did not.
- Shopping cart behavior remained stable during additional exploratory testing.

## Test Environment

- **Application:** nopCommerce Demo Store
- **Environment:** Public Demo
- **Operating System:** Windows 11 Pro 25H2
- **Browser:** Google Chrome 153.0.8010.48
- **Testing Period:** September 2026

The public demo environment may be reset periodically, so test data persistence between testing sessions is not guaranteed.

## Project Status

Testing is complete.

The project includes the full manual QA workflow from planning and test design to execution, defect reporting, exploratory testing, and final reporting.
