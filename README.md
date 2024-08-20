# E-Commerce Back End

[![License](https://img.shields.io/badge/License-MIT_License-green)](http://opensource.org/licenses/MIT)

## Description

The E-Commerce Back End project is a fully functional Express.js API that uses Sequelize to interact with a PostgreSQL database. This project serves as the back end for an e-commerce site, providing RESTful CRUD operations for categories, products, and tags. It allows users to view, create, update, and delete entries in these categories, products, and tags tables. The application is designed to demonstrate the latest technologies and follows the Model-View-Controller (MVC) paradigm.

## Table of Contents

-   [Description](#description)
-   [Functionality](#functionality)
-   [Installation](#installation)
-   [Usage](#usage)
-   [License](#license)
-   [Contributing](#contributing)
-   [Tests](#tests)
-   [Questions](#questions)

## Functionality

This section contains a link to a video that demonstrates the functionality of the E-Commerce Back End application. The video showcases how to set up the database, seed data, and use the API endpoints in Insomnia.

[Watch the walkthrough video here](https://drive.google.com/file/d/1txIcTZLVBN1UYuur33o5p1-6_UmzUjie/view)

## Installation

To set up the E-Commerce Back End application locally, follow these steps:

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/GuillerSaenz/e-commerce-backend.git
    ```

2. Navigate to the project directory:

    ```bash
    cd e-commerce-backend
    ```

3. Install the necessary dependencies:

    ```bash
    npm install
    ```

4. Create a `.env` file in the root directory and add your PostgreSQL credentials:

    ```
    DB_NAME='ecommerce_db'
    DB_USER='your_database_user'
    DB_PASSWORD='your_database_password'
    ```

5. Create the database using the `schema.sql` file:

    ```bash
    psql -U your_database_user -f db/schema.sql
    ```

6. Seed the database with initial data:

    ```bash
    npm run seed
    ```

7. Start the application:

    ```bash
    npm start
    ```

## Usage

The application provides a RESTful API for managing categories, products, and tags. You can use tools like Insomnia or Postman to test the following routes:

-   **Categories**

    -   `GET /api/categories` - Get all categories
    -   `GET /api/categories/:id` - Get category by ID
    -   `POST /api/categories` - Create a new category
    -   `PUT /api/categories/:id` - Update a category
    -   `DELETE /api/categories/:id` - Delete a category

-   **Products**

    -   `GET /api/products` - Get all products
    -   `GET /api/products/:id` - Get product by ID
    -   `POST /api/products` - Create a new product
    -   `PUT /api/products/:id` - Update a product
    -   `DELETE /api/products/:id` - Delete a product

-   **Tags**
    -   `GET /api/tags` - Get all tags
    -   `GET /api/tags/:id` - Get tag by ID
    -   `POST /api/tags` - Create a new tag
    -   `PUT /api/tags/:id` - Update a tag
    -   `DELETE /api/tags/:id` - Delete a tag

## License

This project is licensed under the [MIT License](LICENSE).

## Tests

To test the application manually, follow the steps in the [Usage](#usage) section and ensure all API routes are working as expected. Automated tests can be added in the future.

## Questions

If you have any questions about the project or need further assistance, feel free to reach out:

-   GitHub: [GuillerSaenz](https://github.com/GuillerSaenz)
-   Email: guillersaenzs@gmail.com