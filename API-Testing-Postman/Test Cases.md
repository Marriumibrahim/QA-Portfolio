# API Test Cases

## API Under Test

JSONPlaceholder REST API

Base URL:
https://jsonplaceholder.typicode.com

---

## GET Requests

| ID | Test Scenario | Method | Expected Result |
|---|---|---|---|
| GET-01 | Retrieve a single post | GET | 200 OK and post ID is returned |
| GET-02 | Retrieve posts for a specific user | GET | 200 OK and returned posts belong to requested user |
| GET-03 | Retrieve posts for non-existing user | GET | 200 OK with empty array |
| GET-04 | Retrieve post using environment variable | GET | 200 OK and correct post is returned |

## POST Requests

| ID | Test Scenario | Method | Expected Result |
|---|---|---|---|
| POST-01 | Create a post with valid data | POST | 201 Created |
| POST-02 | Create post without userId | POST | API accepts request and returns created resource |
| POST-03 | Create post with invalid userId type | POST | API behavior is verified |
| POST-04 | Verify JSON response Content-Type | POST | Response Content-Type contains application/json |

## PUT Requests

| ID | Test Scenario | Method | Expected Result |
|---|---|---|---|
| PUT-01 | Update an existing post | PUT | 200 OK |
| PUT-02 | Verify updated title | PUT | Title matches submitted value |
| PUT-03 | Verify updated body | PUT | Body matches submitted value |
| PUT-04 | Verify post ID | PUT | Returned ID matches requested post |

## PATCH Requests

| ID | Test Scenario | Method | Expected Result |
|---|---|---|---|
| PATCH-01 | Partially update post title | PATCH | 200 OK |
| PATCH-02 | Verify updated title | PATCH | Title matches submitted value |
| PATCH-03 | Verify unchanged fields | PATCH | Other fields remain available |

## DELETE Requests

| ID | Test Scenario | Method | Expected Result |
|---|---|---|---|
| DELETE-01 | Delete an existing post | DELETE | 200 OK |
| DELETE-02 | Verify empty response | DELETE | Response is empty |

## Authentication Testing

| ID | Test Scenario | Expected Result |
|---|---|---|
| AUTH-01 | Send request with Bearer token | Authorization header is sent |
| AUTH-02 | Send request without Bearer token | Authorization header is absent |

## Request Chaining

| ID | Test Scenario | Expected Result |
|---|---|---|
| CHAIN-01 | Save post ID from response | postId environment variable is created |
| CHAIN-02 | Use saved post ID in next request | Correct post is retrieved |
