# CoinGecko API Testing Project

## 1. Project Overview

This project focuses on Manual API Testing of the CoinGecko REST API using Postman.

The main objective is to validate API functionality, response data, HTTP status codes, request parameters, headers, error handling, and response time through positive and negative test scenarios.

## 2. Tools & Technologies

- Postman
- JavaScript (Postman Test Scripts)
- CoinGecko REST API
- Git & GitHub

## 3. API Testing Scope

### A. Bitcoin Historical Data API

**Positive Testing**
- HTTP 200 status code validation
- Coin ID, name, and symbol validation
- English localization validation
- Thumbnail URL validation
- Market data validation
- USD and INR current price validation
- USD market capitalization validation
- USD trading volume validation
- Response time validation

**Negative Testing**
- Invalid coin ID
- HTTP 404 status code validation
- Error message validation
- Error code validation
- Error response data type validation

### B. Multiple Coins Market Data API

**Positive Testing**
- HTTP 200 status code validation
- JSON array validation
- Response array length validation
- Bitcoin and Ethereum ID validation
- Coin name and symbol validation
- Currency parameter validation
- Current price and market capitalization validation
- Last updated field validation
- API key header validation
- Accept header validation
- Response time validation

**Negative and Parameter Testing**
- Missing currency parameter
- Invalid currency parameter
- Invalid coin ID
- Empty coin ID
- Missing IDs parameter

### C. Ethereum Historical Data API

**Positive Testing**
- HTTP 200 status code validation
- Price history array validation
- Market capitalization history validation
- Trading volume history validation
- Response data validation
- Timestamp data type validation
- Price data type validation
- Response time validation

**Negative Testing**
- Invalid Ethereum coin ID
- HTTP 404 status code validation
- Error message validation
- Error message data type validation

## 4. Testing Techniques

- Positive Testing
- Negative Testing
- Status Code Validation
- Response Body Validation
- JSON Array and Object Validation
- Data Type Validation
- Query Parameter Validation
- Header Validation
- Error Handling Validation
- Response Time Validation
- Environment Variables
- Postman Collection Runner

## 5. Test Execution Summary

| Metric | Result |
|---|---:|
| Total API Requests | 10 |
| Total Test Assertions | 66 |
| Passed | 66 |
| Failed | 0 |
| Skipped | 0 |
| Average Response Time | 395 ms |
| Execution Duration | 5.385 seconds |

## 6. Project Structure

CoinGecko-API-Testing/
│
├── CoinGecko API Testing.postman_collection.json
│
└── README.md

## 7. How to Execute the Project

Follow these steps to execute the API test collection:

1. Clone or download this repository.
2. Install and open Postman.
3. Click on Import.
4. Import the CoinGecko API Testing.postman_collection.json file from the repository's root directory.
5. Create a Postman Environment named `CoinGecko Environment`.
6. Configure the required environment variables:
   - `coinGeckoApiKey`
   - `ethereumId`
   - `coinId`
   - `testCoin`
7. Add your own valid CoinGecko API key to the `coinGeckoApiKey` variable.
8. Select the CoinGecko Environment in Postman.
9. Open the imported collection.
10. Click Run to execute all requests using Collection Runner.
11. Review the test execution results.

**Note:** Do not upload API keys, tokens, or other secret credentials to GitHub.

## 8. Project Outcome

Successfully executed 10 API requests with 66 passing test assertions and zero failures during collection execution.

This project demonstrates practical experience in API testing, JavaScript assertions, positive and negative testing, environment variables, and Postman Collection Runner.

## 9. Author

- Author: Naveen Kumar
- Project: CoinGecko API Testing
- Tool: Postman
- API Provider: CoinGecko
