StoreAPI
A RESTful API for managing a store built with Node.js, Express, MongoDB, and queryObject, providing CRUD operations.

Create: Add new products to the store with details such as name, company, fields, price, etc.
Read: Retrieve all products or a specific product by ID.
Update: Modify existing product details.
Delete: Remove products from the store.
QueryObject Support: Implement advanced querying capabilities for filtering, sorting, and pagination.
Requirements
Node.js (v14 or later)
MongoDB
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/hirensinh1513/storeAPI.git
cd storeAPI
Install dependencies:

bash
Copy code
npm install
Configuration
Create a .env file in the root directory and add the following environment variables:

env
Copy code
Adjust MONGO_URI to match your MongoDB instance configuration.

Running the Application
Start the application:

bash
Copy code
npm start
The API will be accessible at http://localhost:3000.

API Endpoints
Products
GET /api/products: Get all products.
GET /api/products/
: Get a product by ID.
POST /api/products: Create a new product.
PUT /api/products/
: Update a product by ID.
DELETE /api/products/
: Delete a product by ID.
QueryObject Examples
GET /api/products?name=Apple: Filter products by name (exact match).
GET /api/products?featured=true: Filter products by boolean (exact match).
GET /api/products?price[gte]=10&price[lte]=50: Filter products by price range.
GET /api/products?sort=-price: Sort products by price descending.
GET /api/products?limit=10&page=2: Pagination with 10 products per page, page 2.
Refer to the API documentation for detailed query parameters and examples.
