# API Testing Portfolio

## 1. Project Overview

This project demonstrates API testing techniques using a public demo API.

**Testing Tool:** Postman  
**Protocol:** HTTP/HTTPS  
**Testing Type:** Functional API Testing

### Objectives

- Validate API responses and HTTP status codes.
- Verify response structure and data types.
- Test positive and negative scenarios.
- Validate error handling.
- Document test execution results.

## 2. Test Environment

The project will use the JSONPlaceholder public demo API.

Base URL: https://jsonplaceholder.typicode.com

The API provides sample resources for practising HTTP requests and response validation.

## 3. API Test Scenarios

| Test ID | Endpoint | Method | Scenario | Expected Result |
|---|---|---|---|---|
| API-001 | /posts/1 | GET | Retrieve an existing post | HTTP 200 and a valid post object |
| API-002 | /posts | GET | Retrieve the list of posts | HTTP 200 and a JSON array |
| API-003 | /posts/1/comments | GET | Retrieve comments associated with a post | HTTP 200 and a JSON array |
| API-004 | /posts/999999 | GET | Retrieve a nonexistent post | HTTP 404 or the API's documented not-found response |
| API-005 | /posts | POST | Submit a new sample post | Successful creation response, according to the API's documented behaviour |
| API-006 | /posts/1 | GET | Validate required response fields | The response contains the expected fields and data types |

## 4. Validation Checklist

For each executed request, validate the following where applicable:

- HTTP status code.
- Response body structure.
- Required fields.
- Data types.
- Response headers.
- Response time against an explicitly defined threshold.
- Error handling for invalid requests.

## 5. Test Execution Status

The scenarios above are planned tests.

Execution status should be updated only after running each request and evaluating its response.

JSONPlaceholder simulates data changes rather than permanently storing new or modified records. Results must therefore be interpreted according to the service's documented behaviour.

## 6. Security Considerations

- Use public demo endpoints or an authorised test environment.
- Never commit passwords, API keys, access tokens, or confidential information.
- Do not send sensitive customer data to public testing services.

## 7. Conclusion

This project provides a foundation for API testing using Postman and demonstrates structured scenario design, response validation, and negative testing.
