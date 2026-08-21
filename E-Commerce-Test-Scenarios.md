# E-Commerce Test Scenarios

## Overview

This document contains practical software testing scenarios for an E-Commerce application.

The scenarios cover major customer-facing and backend business processes, including **user registration, product browsing, search, cart management, checkout, payment, order processing, delivery, and order tracking**.

The objective is to validate the functionality, usability, data accuracy, and integration between different components of an E-Commerce system.

---

## E-Commerce Business Flow

**User Registration → Product Search → Product Selection → Cart → Checkout → Payment → Order Confirmation → Order Processing → Delivery → Order Completion**

---

## E-Commerce Test Scenarios

| Test ID  | Test Scenario                                   | Expected Result                                                                                                                |
| -------- | ----------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| ECOM-001 | Register a new customer account                 | Customer account should be created successfully with valid information                                                         |
| ECOM-002 | Register using an existing email address        | System should prevent duplicate account registration                                                                           |
| ECOM-003 | Validate mandatory registration fields          | System should display appropriate validation messages                                                                          |
| ECOM-004 | Login with valid credentials                    | User should be logged in successfully                                                                                          |
| ECOM-005 | Login with invalid credentials                  | System should display an appropriate error message                                                                             |
| ECOM-006 | Test forgot password functionality              | User should be able to reset the password successfully                                                                         |
| ECOM-007 | Browse product categories                       | Relevant products should be displayed correctly                                                                                |
| ECOM-008 | Search for a product using a valid keyword      | Matching products should be displayed                                                                                          |
| ECOM-009 | Search using an invalid/non-existing keyword    | System should display an appropriate no-result message                                                                         |
| ECOM-010 | Apply product filters                           | Products should be filtered according to selected criteria                                                                     |
| ECOM-011 | Apply product sorting                           | Products should be sorted according to the selected option                                                                     |
| ECOM-012 | View product details                            | Product information, price, images, stock status, and other details should be displayed correctly                              |
| ECOM-013 | Add an available product to cart                | Product should be added to the shopping cart                                                                                   |
| ECOM-014 | Increase product quantity in cart               | Cart quantity and total price should update correctly                                                                          |
| ECOM-015 | Decrease product quantity in cart               | Cart quantity and total price should update correctly                                                                          |
| ECOM-016 | Remove a product from cart                      | Selected product should be removed and cart total should update                                                                |
| ECOM-017 | Add an out-of-stock product to cart             | System should prevent purchase or display the correct stock message                                                            |
| ECOM-018 | Verify cart subtotal                            | Cart subtotal should be calculated accurately                                                                                  |
| ECOM-019 | Apply a valid discount/promo code               | Applicable discount should be applied correctly                                                                                |
| ECOM-020 | Apply an invalid or expired promo code          | System should reject the code and display an appropriate message                                                               |
| ECOM-021 | Proceed to checkout with valid cart items       | User should be able to proceed to checkout                                                                                     |
| ECOM-022 | Validate shipping address                       | System should accept valid address information and reject invalid data                                                         |
| ECOM-023 | Select delivery/shipping method                 | Selected delivery method and applicable charge should be reflected correctly                                                   |
| ECOM-024 | Verify order total before payment               | Product price, discount, shipping charge, tax, and final amount should be calculated correctly                                 |
| ECOM-025 | Complete payment successfully                   | Payment should be processed and order should be created successfully                                                           |
| ECOM-026 | Test failed payment scenario                    | Order/payment status should be handled correctly without incorrect deduction                                                   |
| ECOM-027 | Prevent duplicate order submission              | Multiple orders should not be created from a single transaction                                                                |
| ECOM-028 | Verify order confirmation                       | Customer should receive correct order confirmation details                                                                     |
| ECOM-029 | Verify order status                             | Order status should update correctly throughout the order lifecycle                                                            |
| ECOM-030 | Verify inventory after successful order         | Purchased quantity should be deducted correctly from available stock                                                           |
| ECOM-031 | Verify order processing                         | Admin/system should be able to process the order successfully                                                                  |
| ECOM-032 | Verify order shipment                           | Shipment information should be recorded correctly                                                                              |
| ECOM-033 | Verify order tracking                           | Customer should be able to view the correct order/shipment status                                                              |
| ECOM-034 | Cancel an eligible order                        | Eligible order should be cancelled successfully                                                                                |
| ECOM-035 | Prevent cancellation of a non-cancellable order | System should prevent cancellation according to business rules                                                                 |
| ECOM-036 | Verify refund process                           | Refund should be processed according to the applicable payment and order rules                                                 |
| ECOM-037 | Verify customer order history                   | Customer should be able to view previous orders with accurate information                                                      |
| ECOM-038 | Verify admin product management                 | Authorized admin should be able to add, edit, and manage products                                                              |
| ECOM-039 | Verify product stock management                 | Product stock quantity should be updated accurately                                                                            |
| ECOM-040 | Verify end-to-end E-Commerce workflow           | Customer, product, cart, payment, inventory, order, and delivery data should remain consistent throughout the complete process |

---

## Key Testing Areas

### Functional Testing

* User registration and login
* Product browsing
* Product search
* Product filtering and sorting
* Product details
* Shopping cart
* Checkout
* Discount/promo code
* Payment
* Order management
* Delivery
* Order tracking
* Cancellation and refund

### Integration Testing

The following integrations should be validated:

* Product ↔ Inventory
* Cart ↔ Product
* Cart ↔ Checkout
* Checkout ↔ Payment
* Payment ↔ Order
* Order ↔ Inventory
* Order ↔ Delivery
* Delivery ↔ Order Tracking

### Data Validation

Important data points to validate include:

* Product price
* Product stock
* Cart quantity
* Discount amount
* Shipping charge
* Tax
* Order total
* Payment status
* Order status
* Inventory quantity
* Refund amount

---

## Positive Testing

Examples:

* Register with valid information
* Login with valid credentials
* Search for an existing product
* Add an available product to cart
* Apply a valid promo code
* Complete checkout with valid information
* Complete successful payment
* Track a valid order

---

## Negative Testing

Examples:

* Register with an existing email
* Login with invalid credentials
* Search for a non-existing product
* Add an unavailable product to cart
* Enter invalid shipping information
* Apply an expired promo code
* Submit invalid payment information
* Attempt duplicate order submission
* Attempt to cancel a non-cancellable order

---

## End-to-End Testing

The complete E-Commerce workflow should be validated from:

**Customer Registration → Product Search → Product Selection → Cart → Checkout → Payment → Order Creation → Inventory Update → Order Processing → Shipment → Delivery → Order Completion**

The purpose is to ensure that every transaction remains consistent across the customer-facing and backend components of the application.

---

## Testing Approach

For E-Commerce application testing, I focus on:

1. Requirement Analysis
2. Business Flow Analysis
3. Test Scenario Preparation
4. Functional Testing
5. Positive Testing
6. Negative Testing
7. Integration Testing
8. Data Validation
9. Regression Testing
10. End-to-End Testing
11. Defect Identification and Reporting
12. Business Rule Validation

---

## Skills Demonstrated

* E-Commerce Application Testing
* Functional Testing
* Integration Testing
* End-to-End Testing
* Regression Testing
* Positive & Negative Testing
* Test Scenario Design
* Business Flow Validation
* Data Validation
* Defect Identification
* Requirement Analysis
* Cross-Module Testing

---

**Note:** This portfolio contains generic testing scenarios. Client-specific confidential information, credentials, internal URLs, and sensitive business data have been excluded.
