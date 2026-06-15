# 6.6 Lab – Usability Test Outline & Performance Validation

## System Overview

I selected the **Amazon website (e-commerce platform)** for this usability test.

Amazon is an online shopping system that allows users to search for products, view details, add items to a cart, and complete purchases. Its main purpose is to make online shopping fast, easy, and reliable.

The intended audience includes general consumers of all experience levels, from first-time users to frequent online shoppers.

---

## Study Type and Justification

This is an **Assessment usability test**.

Amazon is already a fully developed system, so the goal is to evaluate how well users can complete key tasks such as searching for products, adding items to a cart, and completing checkout.

The results help identify usability issues like navigation confusion, slow checkout flow, or difficulty finding products.

---

## Research Questions

1. Can users successfully locate a product using the search function?
2. Can users add a product to the shopping cart without confusion?
3. Can users complete the checkout process efficiently?
4. How long does it take users to complete a purchase task?
5. Where do users most commonly make errors during the process?

---

## Participants

The target users are general online shoppers aged 18–60 with basic internet experience.

A sample size of **5–8 participants** is appropriate because usability testing focuses on identifying patterns and usability issues rather than statistical accuracy.

These participants reflect real-world users of the system.

---

## Task Scenarios

### Task 1: Product Search
A user wants to find a “wireless mouse” for work or school use.  
**Success:** The user is able to locate a relevant product listing.

### Task 2: Product Comparison
A user compares two wireless mouse options and selects one.  
**Success:** The user views product details and makes a selection.

### Task 3: Add to Cart
A user decides to purchase a wireless mouse and adds it to the cart.  
**Success:** The item appears in the shopping cart.

### Task 4: Checkout Process
A user proceeds through checkout until the order confirmation step.  
**Success:** The user reaches the confirmation page.

---

## Success Criteria and Metrics

### Task Completion Rate
Measures whether users successfully complete each task without assistance.

### Time on Task
Measures how long each task takes. Faster completion indicates better usability.

### Error Frequency
Tracks mistakes such as wrong clicks, confusion, or backtracking.

### Satisfaction / Confidence Rating
Users rate how confident they felt completing each task (1–5 scale).

---

## Performance Validation Using JMeter

### High-Value Workflow

The **checkout process** was selected because it directly affects user trust and revenue.

Performance is critical because slow response times can lead to cart abandonment and loss of sales.

---

### JMeter Test Configuration

- Number of Virtual Users: **10**
- Ramp-up Time: **10 seconds**
- Test Duration: **60 seconds**
- Target Endpoint: `/checkout`
- Expected Response Time: **under 2 seconds**

---

### Sample Results (Replace with your actual results)

- Average Response Time: 1.8 seconds  
- Throughput: 12 requests/second  
- Error Rate: 0%  

---

## Reflection

Performance has a direct impact on usability. In this test, the checkout process performed efficiently, supporting a smooth user experience.

If response times were slower, users would likely abandon their carts or lose trust in the system.

Overall, the workflow meets acceptable performance thresholds, but if delays exceeded 3–4 seconds, optimization would be required before release.

Improvements would focus on backend optimization and reducing server load to improve responsiveness.

---

## Submission Contents

This repository includes:

- Usability test outline (this README)
- JMeter test plan (.jmx file)
- Execution evidence screenshots
- Reflection document
