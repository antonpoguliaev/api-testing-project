# Bug Reports

## Bug Report 1

Title: API returns empty object for non-existing user

Endpoint:
GET /users/999

Steps to reproduce:
1. Send GET request to /users/999

Expected result:
API should return 404 Not Found

Actual result:
API returns status 200 with empty object

Severity: Low
Priority: Low
