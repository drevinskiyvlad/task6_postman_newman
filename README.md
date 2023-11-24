# Postman + Newman (Simple Store Template)

## Summary of Repo

This repository provides a simple template for testing REST APIs using Postman, Newman. The main
focus is on local server testing with a provided API, but you can easily adapt it to test other APIs using Postman
collections. The repository includes documentation and automated workflows for GitHub Actions to streamline the testing
process.

## Requirements

- Node.js (npm)
- Postman (for integration tests)

## Steps to Install

1. Clone this repository:
2. Install Node.js dependencies:
   ```bash
   npm install
   ```
3. Run the testing server locally:
   ```bash
   npm run tern-on-api
   ```

## Steps to Launch

1. Upload `store.collection.json` in the Postman app.

2. Run the integration tests in Postman.

### Overview of Local Server Testing

The local server provides three routes: `/products`, `/orders`, and `/users`. Each route supports various operations, as
detailed in the table below using the example resource `products`.

| VERB   | Route         | Input       | Output             |
|--------|---------------|-------------|--------------------|
| GET    | /products     | *None*      | **Array**          |
| GET    | /products/:id | **e.g., 3** | **Object**         |
| POST   | /products     | **object**  | **Created object** |
| PUT    | /products     | **object**  | **Updated object** |
| DELETE | /products/:id | **e.g., 3** | **Deleted object** |