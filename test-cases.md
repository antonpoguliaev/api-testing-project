# API Test Cases

## Test Case 1

Title: Get user by ID

Endpoint:
GET /users/1

Steps:
1. Send GET request to /users/1

Expected result:
Status code: 200 OK  
Response body contains user object with id = 1

## Test Case 2

Title: Verify API returns correct user data structure

Endpoint:
GET /users/1

Steps:
1. Send GET request to /users/1

Expected result:
Status code: 200 OK

Response body contains fields:
- id
- name
- username
- email
- address
- phone
- website
- company

Field types:
- id → number
- name → string
- email → string

## Test Case 3

Title: Verify API returns 404 for non-existing user

Endpoint:
GET /users/999

Steps:
1. Send GET request to /users/999

Expected result:
Status code: 404 Not Found
Response body indicates that user does not exist
