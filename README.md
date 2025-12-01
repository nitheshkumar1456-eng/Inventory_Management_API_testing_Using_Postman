# Inventory Management API – Postman Collection

This project contains a Postman collection for testing, validating, and visualizing an Inventory Management API. It includes CRUD operations, environment variables, advanced test scripts, and visualizers.

## 1. Introduction

The Inventory Management API is a RESTful service designed to manage product information efficiently. It allows adding, retrieving, updating, and deleting product records. The project demonstrates automated testing using Postman and Newman.

## 2. API Overview & Architecture

* **Base URL:** [https://692ab9037615a15ff24d790a.mockapi.io](https://692ab9037615a15ff24d790a.mockapi.io)
* **Endpoint:** /Products

### CRUD Operations:

* **GET /Products:** Retrieve all products.
* **POST /Products:** Add a new product.
* **GET /Products/{ProductID}:** Retrieve a product by ID.
* **PUT /Products/{ProductID}:** Update a product by ID.
* **DELETE /Products/{ProductID}:** Delete a product by ID.

### Environment Variables:

* `baseURL` - API base URL
* `endpoint` - Resource endpoint
* `ProductID` - Dynamic product ID
* `ID` - Additional ID for deletion
* `ProductName` - Product name input
* `Suppliers` - Supplier name
* `Stocks` - Boolean stock status

### API Architecture:

* RESTful design with stateless communication.
* JSON data model.
* MockAPI backend simulates real-world API behavior.

## 3. Postman Collection Design

* Structured requests for all CRUD operations.
* Test scripts for status codes, headers, schema, and response times.
* Visualizers for product tables, stock distribution charts, and product detail cards.

## 4. Newman and HTML Extra Reporter

Newman is a command-line tool to run Postman collections. It supports automation and integration with CI/CD pipelines:

```
npm install -g newman
newman run Inventory_management.postman_collection.json
```

Newman HTML Extra generates detailed and interactive HTML reports:

```
npm install -g newman-reporter-htmlextra
newman run Inventory_management.postman_collection.json -r htmlextra
```

## 5. Test Results & Visual Output

* Product tables and stock distribution charts in Postman visualizer.
* Product detail cards for GET and PUT requests.
* Newman CLI outputs and HTML reports for automated test results.

## 6. Conclusion

The Inventory Management API project demonstrates effective API testing using Postman and Newman. It provides automation, structured testing, and professional reports, making it suitable for developers, QA engineers, and CI/CD workflows.

**🚀 The Newman HTML Extra report has been successfully deployed in this repository for easy access and review.**
