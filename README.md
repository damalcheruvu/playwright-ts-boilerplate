# 🎭 Playwright Boilerplate Framework for EU&C POC

## Introduction

This repository provides a robust framework for automating end-to-end tests for web applications using Playwright and Typescript. It also includes support for API testing, making it a comprehensive solution.

## Tech Details

- **Playwright**: A cross-browser automation library for Node.js. It enables you to write reliable end-to-end tests for web applications and websites. With Playwright, you can automate scenarios across multiple browsers (Chromium, Firefox, WebKit) and platforms (Windows, Linux, macOS).
- **Allure**: A flexible, lightweight multi-language test report tool that provides a concise representation of test results in a neat web report form. It allows everyone participating in the development process to extract maximum useful information from everyday execution of tests.

[Playwright Documentation](https://playwright.dev/)

## Prerequisites

- Node.js (>= 20.x)
- pnpm (>= 9.x) or npm
- Docker (for containerized execution)

## Setup Instructions

   ```bash
   npm install
   ```

## Running Tests

To run the tests, use the following command:

```bash
npm run test:playwright
```

## API Testing with Playwright

This repository now includes support for testing REST APIs using Playwright. You can use the provided helper functions to perform HTTP GET, POST, and PATCH requests, and write your own API tests.

### Helper Functions

The following helper functions are available in `src/core/apiHelpers.ts`:

- `HttpGet(url: string, headers?: Record<string, string>)`: Perform an HTTP GET request.
- `HttpPost(url: string, data: any, headers?: Record<string, string>)`: Perform an HTTP POST request.
- `HttpPatch(url: string, data: any, headers?: Record<string, string>)`: Perform an HTTP PATCH request.

### Sample API Tests

Sample API tests are available in `src/tests/api.test.spec.ts`. These tests demonstrate how to use the helper functions to perform API requests and validate the responses.
