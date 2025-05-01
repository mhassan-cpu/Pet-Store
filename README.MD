# Swagger Petstore API

![Swagger Petstore](Download.png)

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Available Endpoints](#available-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Swagger Petstore is a demo API designed to illustrate the capabilities of Swagger/OpenAPI. It allows users to perform CRUD operations on pets, manage store orders, and user accounts. The API is commonly used for testing, automation practice, and API documentation learning.

## Local Testing Execution Example

![Local Testing Execution Example](Example.gif)

## Features

- **Add Pet**: Add a new pet to the store.
- **Retrieve Pet(s)**: Retrieve pet details by ID or by status.
- **Update Pet**: Fully update an existing pet record.
- **Delete Pet**: Delete a pet by ID.
- **Manage Users**: Create, update, retrieve, and delete user accounts.
- **Store Operations**: Place and manage pet orders.

## Installation

To set up the Swagger Petstore API locally (optional), follow these steps:

Clone the repository:

```bash
git clone https://github.com/mhassan-cpu/Pet-Store.git
```

Navigate to the project directory:

```bash
cd Pet-Store-platform
```

Install dependencies (using Maven or Node.js if applicable for your setup):

For Node.js mock server:

npm install

Configure the application:

Set up any environment variables if needed (e.g., database, ports).

Run the application:

For Node.js server:

npm start

Run the application:

```bash
npm start
```

## Usage

You can interact with the API using tools like:
- **Postman**
- **Newman**
- **cURL**
- **Automation frameworks** (e.g., Cypress, Rest Assured, etc.)

Most operations are publicly accessible and don’t require authentication. However, login/logout simulation is provided.

## Available Endpoints

### Pet APIs

- `GET /pet/{petId}` : Retrieve a pet by ID.
- `POST /pet` : Add a new pet.
- `PUT /pet` : Update an existing pet.
- `DELETE /pet/{petId}` : Delete a pet.
- `GET /pet/findByStatus` : Filter pets by status.

### Store APIs

- `GET /store/inventory` : Get inventory by status.
- `POST /store/order` : Place a new order.
- `GET /store/order/{orderId}` : Retrieve order by ID.
- `DELETE /store/order/{orderId}` : Delete order by ID.

### User APIs

- `POST /user` : Create a new user.
- `GET /user/{username}` : Retrieve user by username.
- `PUT /user/{username}` : Update a user.
- `DELETE /user/{username}` : Delete a user.
- `GET /user/login` : Log user in.
- `GET /user/logout` : Log user out.

## Example Request - Add Pet

```bash
POST /pet
Content-Type: application/json

{
  "id": 123,
  "category": {
    "id": 1,
    "name": "Dogs"
  },
  "name": "Rex",
  "photoUrls": [
    "https://example.com/rex.jpg"
  ],
  "tags": [
    {
      "id": 1,
      "name": "friendly"
    }
  ],
  "status": "available"
}
```

## Contributing

We welcome contributions for:
- Enhancing API documentation
- Adding sample test cases or scripts
- Improving usage examples

### Steps to Contribute
1. Fork the repository.
2. Create a feature branch.
3. Submit a pull request.

## License

Swagger Petstore is public and available freely for demo, education, and testing purposes.

---

> ✨ Happy API Testing with Swagger Petstore! ✨

