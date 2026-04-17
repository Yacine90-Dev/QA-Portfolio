# API Testing Project - JSONPlaceholder

## 📌 Objective
This project demonstrates API testing skills using Postman on a public REST API.

## 🛠 Tools Used
- Postman
- JSONPlaceholder API

## 🔍 Test Scenarios

### 1. Get Post by ID
- Endpoint: /posts/1
- Method: GET
- Validates:
  - Status code 200
  - Response structure
  - Correct data (id, userId)
  - Non-empty title

### 2. Create Post
- Endpoint: /posts
- Method: POST
- Validates:
  - Status code 201
  - Response contains created resource

### 3. Get Non-existing Post
- Endpoint: /posts/101
- Method: GET
- Validates:
  - Status code 404

## 📊 Key Learnings
- API request handling (GET, POST)
- JSON validation
- Automated testing with Postman scripts
- Understanding of fake vs real APIs
- QA Analysis

During testing, it was observed that the POST request returns a 201 status and a new ID.  
However, this API does not persist data, as a subsequent GET request on the new resource returns a 404 status.

This indicates that JSONPlaceholder is a mock API used for testing purposes.

## 📁 Project Structure
- Postman Collection (JSON file)
- README documentation
