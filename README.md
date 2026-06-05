# POM-Automation-Framework

# Playwright Test Automation Framework

## Overview
- **Tech:** Playwright, TypeScript, Page Object Model (POM)
- **Scope:** E2E testing for legacy government web system
- **Scale:** 500+ test cases across 77 change requests

## Project Structure
├── library/                    # Page Object Model classes
│   ├── pages/
│   │   ├── BasePage.ts        # Base page with waits, assertions, utilities
│   │   ├── LoginPage.ts
│   │   └── DashboardPage.ts
│   ├── actions/               # Reusable action helpers
│   └── data/                  # Test data builders
├── tests/
│   └── 02-automate/           # Test specifications (.spec.ts)
├── playwright.config.ts       # Playwright configuration
├── package.json               # Dependencies
└── README.md

## Key Features
- **Custom Utilities:** Retry logic, page reload recovery, smart wait strategies
- **Resilient Selectors:** XPath/CSS for dynamic IDs, slow responses
- **CI/CD Integration:** Jenkins pipelines for scheduled execution
- **Data-Driven Testing:** Support for CSV/JSON/XLSX test data

## Running Tests
```bash
npm install
npx playwright test
```
