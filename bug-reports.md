# Bug Reports

## Bug Report 1

Title: API allows creating post with empty title field

Endpoint:
POST /posts

Steps to reproduce:
1. Send POST request to /posts
2. Use request body:

{
  "title": "",
  "body": "testing API",
  "userId": 1
}

Expected result:
API should validate input data and return an error response (400 Bad Request).

Actual result:
API creates a post successfully and returns status code 201.

Severity: Medium  
Priority: Medium
