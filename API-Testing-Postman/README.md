# API Testing with Postman

## Project Overview

This project demonstrates manual API testing using Postman against the JSONPlaceholder REST API.

The project covers CRUD operations, response validation, status code verification, header validation, environment variables, positive and negative testing, and request chaining.

## Application Under Test

**JSONPlaceholder**

A free fake REST API used for testing and development.

**Base URL:**  
https://jsonplaceholder.typicode.com

## Tools & Technologies

- Postman
- JavaScript
- REST API
- JSON
- GitHub

## Testing Covered

### HTTP Methods

- GET
- POST
- PUT
- PATCH
- DELETE

### Validation

- HTTP status codes
- Response body
- Response properties
- Response headers
- Content-Type
- Empty responses
- JSON response structure

### API Testing Techniques

- Positive testing
- Negative testing
- Query parameter testing
- Environment variables
- Request chaining
- Bearer token/header validation

## Test Scenarios

| Area | Scenarios |
|---|---|
| GET | Retrieve single post, filter posts by user |
| POST | Create post and validate response |
| PUT | Replace existing post |
| PATCH | Partially update post |
| DELETE | Delete post and validate response |
| Authentication | Validate presence/absence of Bearer token |
| Request Chaining | Extract ID and reuse it in another request |

## Postman Collection

The complete Postman collection is included in this repository:

`API-Testing-JSONPlaceholder.postman_collection.json`

It contains executable requests and Postman test scripts.

## Test Cases

Detailed test scenarios and expected results are documented in:

`Test-Cases.md`

## Key Skills Demonstrated

- REST API testing
- Postman
- Test case design
- JavaScript assertions
- API response validation
- Positive and negative testing
- Environment variable management
- Request chaining
- Defect-oriented thinking
- QA documentation

- ## Test Execution Summary

All documented API requests were executed in Postman and validated using Postman test scripts.

| Request | Result |
|---|---|
| GET - Single Post | PASS |
| GET - Posts by User | PASS |
| POST - Create Post | PASS |
| PUT - Update Post | PASS |
| PATCH - Update Post | PASS |
| DELETE - Delete Post | PASS |
| GET - Request Chaining | PASS |

### Overall Result

**7/7 API request scenarios passed successfully.**
