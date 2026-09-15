# Test Plan - nopCommerce QA Project

## 1. Project Overview

**Application:** nopCommerce Demo Store

**Testing Type:** Independent Black-box QA Assessment

## 2. Objective

The goal of this project is to check the quality of the nopCommerce e-commerce application, make sure its main features work as expected, and verify that users can complete a purchase without problems.

## 3. Scope

### Authentication & Account Management
- User registration
- Login and logout
- Password recovery
- Account-related functionality

### Product Discovery
- Product catalog
- Product search
- Categories
- Filters
- Sorting
- Product details

### Shopping Cart
- Add products to cart
- Remove products from cart
- Change product quantity
- Verify cart contents and totals

### Checkout & Payment
- Checkout flow
- Customer and shipping information
- Payment method
- Order placement

### Order Management
- Order confirmation
- Order history
- Order status

## 4. Out of Scope

- Performance testing
- Load testing
- Security testing
- Mobile application testing
- Third-party payment gateway internals
- Admin panel functionality

## 5. Test Types

- Smoke Testing
- Functional Testing
- UI Testing
- Negative Testing
- Exploratory Testing
- Regression Testing
- End-to-End Testing

## 6. Test Environment

**Application:** nopCommerce Demo Store

**Environment:** Public Demo

**Operating System:** Windows 11 Pro, Version 25H2

**Browser:** Google Chrome, Version 153.0.8010.48

**Testing Date:** September 2026

**Note:** The application is a public demo environment and may be reset or changed between test sessions.

## 7. Test Data

### User Account Data
- Valid user account
- Invalid email addresses
- Invalid passwords
- Empty required fields

### Product Data
- Available products
- Products from different categories
- Products from different manufacturers
- Products with different prices and quantities

### Checkout Data
- Valid customer information
- Invalid and incomplete customer information
- Valid test payment card number
- Invalid card numbers

### Search and Filter Data
- Existing product names
- Non-existing product names
- Valid and invalid filter combinations

**Note:** Only test data is used during testing. No real payment or personal data is stored in the project.

## 8. Risks and Priorities

### High Priority
- Registration
- Login and logout
- Password recovery
- Product search
- Shopping cart
- Checkout and payment
- Order placement

Issues in these areas can prevent users from accessing their accounts or completing a purchase.

### Medium Priority
- Product filters and sorting
- Product details
- Order history

Issues in these areas may affect the user experience but may not always prevent the user from completing a purchase.

### Low Priority
- Minor UI issues
- Cosmetic issues
- Non-critical information display

These issues have a lower impact on the main customer journey and purchase process.
