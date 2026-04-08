# QA Portfolio – Rozetka Testing

## 📌 Project Description

Manual testing of a large-scale e-commerce web application with focus on real user scenarios, edge cases, and system behavior.

---

## 🔍 Scope

* Authentication (Login/Registration)
* Product Catalogue
* Product Page
* Cart
* Checkout

---

## 🧪 Testing Types

* Functional testing (Checklist-based, Exploratory)
* Specification-based testing:

  * Equivalence Partitioning
  * Boundary Value Analysis
  * State Transition Testing
* UI/UX testing

---

## 🛠 Tools Used

* Manual testing techniques
* Chrome DevTools (Elements, Network)
* Basic API analysis
* Postman (in progress)

---

## 📂 Artifacts

* Test Cases -> `/test-cases`
* Checklists -> `/checklists`
* Bug Reports -> `/bug-reports`
* Evidence (screenshots, gifs) -> `/evidence`
* Network Analysis -> `/network-analysis`

---

## 🔍 Key Findings

* UI issues affecting usability (header, filters, responsive behavior)
* Performance issue caused by lack of input validation (large input handling)
* Broken external link in consent flow
* Inconsistency between UI and API (discount not reflected in UI)
* Potential user enumeration issue during authentication

---

## 🌐 Network & API Insights

* API returns HTTP 200 for both successful and failed login attempts
* Error handling is implemented via response body instead of HTTP status codes
* Cart functionality relies on multiple API calls:
  * cart state
  * UI blocks
  * additional services
* Multiple API calls are used to update cart, which may lead to inconsistent UI state if one of the requests fails

---

## 🧠 Notes

Testing was performed manually with focus on:
* Positive / Negative scenarios
* Edge cases
* Real user behavior
* UI and backend interaction analysis
