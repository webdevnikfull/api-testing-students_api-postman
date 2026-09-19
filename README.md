# 🧪 QA Automation Portfolio: Students API Testing & Automation

> About this repository: This project demonstrates automated API testing using Postman and JavaScript test scripts (Chai assertions) for the Mate Academy Students API. It covers data retrieval endpoints for goods and filtered todo items by user ID and completion status[cite: 23]. It also highlights a modern "Shift-Left" QA approach and Continuous Integration (CI/CD) readiness via Newman.

![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Newman](https://img.shields.io/badge/Newman-026E42?style=for-the-badge&logo=postman&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

## 🎯 Project Overview

This collection provides automated API test scripts targeting the Students API endpoints (`https://mate.academy/students-api`)[cite: 23]. It validates product listings and user-specific todo filtering workflows.

As a QA Automation / API Testing Engineer, my focus in this repository is to implement clean automated assertions, verify query parameter filtering, and ensure reliable REST API contract validation.

## 🛠️ QA Tech Stack & Tools

* **API Testing Tool:** Postman
* **CLI Runner / CI Execution:** Newman
* **Test Assertions & Scripting:** JavaScript (Chai Assertion Library built into Postman)
* **CI/CD Pipeline Support:** GitHub Actions
* **Target Environment:** Mate Academy Students API[cite: 23]

## 📊 Test Strategy & Coverage

### 1. Automated API Testing & Assertions
The Postman collection includes structured test suites (`pm.test`) validating:
* **All goods (`GET /students-api/goods`):** Verifies successful retrieval of the complete goods list, expecting an HTTP 200 OK status[cite: 23].
* **Goods by ID (`GET /students-api/goods/245`):** Validates retrieval of specific item details by ID, expecting an HTTP 200 OK status[cite: 23].
* **Todo Filtering by User & Status (`GET /students-api/todos?userId=...&completed=...`):** Tests query parameter filtering for specific users (e.g., user `1044` with completed `FALSE`, and user `4308` with completed `TRUE`), verifying correct response handling with an HTTP 200 OK status[cite: 23].

## 🚀 How to Run the Tests Locally

To run and evaluate this Postman collection locally using Node.js and Newman, follow these steps:

### 1. Prerequisites
Ensure you have Node.js installed, then install Newman globally (if not already installed):
```bash
npm install -g newman
