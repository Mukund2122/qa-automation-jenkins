# QA Automation Assignment - Playwright & Jenkins

## Project Overview
This repository contains a suite of 5 automated test cases for the [SauceDemo](https://www.saucedemo.com/) web application, integrated into a CI/CD pipeline using Jenkins.

## Tech Stack
* **Framework:** Playwright (JavaScript)
* **CI/CD:** Jenkins
* **Test Site:** SauceDemo (E-commerce flow)

## Included Test Cases
1. **Successful Login:** Validates access with standard credentials.
2. **Failed Login:** Validates error handling for incorrect credentials.
3. **Add to Cart:** Verifies product selection and cart badge updates.
4. **Navigation:** Ensures item detail pages load correctly.
5. **Logout:** Confirms secure session termination.

## How to Run Locally
1. Clone the repository.
2. Install dependencies: `npm install`
3. Install browsers: `npx playwright install`
4. Run tests: `npx playwright test`

## CI/CD Integration
The `Jenkinsfile` in the root directory defines a declarative pipeline with four stages: Checkout, Environment Setup, Automation Execution, and Reporting. It is designed to run on any Jenkins agent with Node.js installed.