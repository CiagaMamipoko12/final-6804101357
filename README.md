# Playwright Final Exam

## Project Overview

This project contains automated tests for the [SauceDemo](https://www.saucedemo.com/) web application using Playwright Test and TypeScript.

## Technologies Used

- Playwright Test
- TypeScript
- Node.js
- Chromium

## Project Structure

```text
final-exam/
├── README.md
├── package.json
├── package-lock.json
├── playwright.config.ts
├── tests/
│   ├── unit/
│   │   ├── UT-01.spec.ts
│   │   └── UT-02.spec.ts
│   ├── integration/
│   │   ├── IT-01.spec.ts
│   │   └── IT-02.spec.ts
│   └── system/
│       ├── ST-01.spec.ts
│       └── ST-02.spec.ts
├── playwright-report/
│   └── index.html
└── reports/
    ├── results.json
    └── test-summary.md
```

## Test Suites

### Unit Tests
- **UT-01:** Login form validation
- **UT-02:** Product button state changes between Add to Cart and Remove

### Integration Tests
- **IT-01:** Top-down integration using a real login flow and a browser-level inventory stub
- **IT-02:** Driver-based login state followed by testing the real inventory and cart

### System Tests
- **ST-01:** Complete purchase of two products
- **ST-02:** Checkout validation and recovery

## Installation

Install project dependencies:

```bash
npm install
```

Install Playwright browsers if needed:

```bash
npx playwright install
```

## Running Tests

Run all tests:

```bash
npx playwright test
```

Open the HTML report:

```bash
npx playwright show-report
```

## Test Reports

The project generates the following reports after a test run:

- `playwright-report/index.html` — HTML test report
- `reports/results.json` — machine-readable JSON test results
- `reports/test-summary.md` — summary of test results

The test summary should reflect the actual results of the corresponding test run.

## Latest Recorded Test Result

The latest result recorded during project development was:

- Passed: 8
- Failed: 0
- Skipped: 0
- Flaky: 0

See `reports/test-summary.md` and the generated HTML report for the recorded results.

## Application

SauceDemo: https://www.saucedemo.com/
