# Kishan-Andolan QA Testing

This directory contains the testing documentation and resources for the Kishan-Andolan project.

## Testing Structure

The testing process is divided into two phases:

1. **Soft Testing** - Manual testing of UI, functionality, and user flows
2. **Hard Testing** - Technical testing including API testing, performance testing, and security assessment

## Directory Structure

```
qa-reports/
├── README.md (this file)
├── create_excel_file.ps1 (script to generate Excel checklist file)
├── soft-testing/
│   ├── bugs.md (documentation of bugs found during soft testing)
│   └── check_lists_soft_hard.xlsx (test cases and results for both soft and hard testing)
└── hard-testing/
    ├── api-tests/
    │   └── postman_collection.json (Postman collection for API testing)
    ├── performance-logs/
    │   └── load-test-report.csv (performance test results)
    └── security-report.md (security testing findings)
```

## Getting Started

### Soft Testing

Use the `soft_testing` sheet to track:
- UI testing on different devices and browsers
- Functionality testing of all features
- User flow testing

Document any bugs found in `bugs.md`.

### Hard Testing

#### API Testing
1. Import the Postman collection from `hard-testing/api-tests/postman_collection.json`
2. Set up your environment variables (baseUrl, authToken, etc.)
3. Run the tests and document results in the Excel file

#### Performance Testing
1. Used tools like JMeter to run load tests
2. Save the results in `hard-testing/performance-logs/load-test-report.csv`
3. Document findings in the Excel file

#### Security Testing
1. Perform security testing using tools like OWASP ZAP, Burp Suite, etc.
2. Document findings in `hard-testing/security-report.md`

## QA Sign-off

Use the `QA_SignOff` sheet to track the final verification and sign-off of all requirements before release. 