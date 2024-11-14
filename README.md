E-commerce Backend
This repository hosts the backend for an e-commerce platform, developed with Node.js and Express. The backend supports user authentication, product management, cart handling, and order processing.

Features
User Authentication: Register and log in with secure password hashing and token-based authentication.
Product Management: Add, update, delete, and view products in the catalog.
Cart Management: Add products to cart, update quantities, and view cart details.
Order Management: Place orders and view past orders.
Prerequisites
Node.js (version 14 or higher)
MongoDB (running locally or remotely)
npm (Node Package Manager)
Getting Started
Clone the Repository
Clone the repository and navigate to the project directory:

git clone https://github.com/Raghav973171/ecommerce-backened.git
cd ecommerce-backened
Environment Configuration
Create a .env file in the project root directory with the following variables:

# MongoDB Configuration
MONGODB_URI=mongodb://localhost:27017/ecommerce_db

# JWT Secret Key
JWT_SECRET=your_secret_key

# Server Port
PORT=5000
Ensure MongoDB is running locally or configure MONGODB_URI with your remote database connection string.

Install Dependencies
Install the necessary Node.js dependencies:

npm install
Run the Application
Start the server:

npm start
The server will start on http://localhost:5000 or on the port specified in .env.

API Documentation
Authentication
Sign Up: POST /signup - Register a new user.
Sign In: POST /signin - Log in an existing user.
Product Management
Add Product: POST /addproduct - Add a new product.
Update Product: PUT /updateproduct/:productId - Update details for an existing product.
Delete Product: DELETE /deleteproduct/:productId - Remove a product from the catalog.
Get All Products: GET /products - Retrieve the full product catalog.
Cart Management
Add Product to Cart: POST /cart/add - Add a product to the user’s cart.
Update Cart: PUT /cart/update - Update quantities in the cart.
Delete Product from Cart: DELETE /cart/delete - Remove an item from the cart.
Get Cart: GET /cart - View current cart contents.
Order Management
Place Order: POST /placeorder - Process and place an order for the items in the cart.
Get All Orders: GET /getallorders - Admin view to retrieve all orders.
Get Orders by Customer: GET /orders/customer/:customerId - Retrieve orders for a specific customer.
Running Tests
To run tests (assuming a test framework is set up):

npm test
Build and Deployment
To prepare the app for deployment, use the following:

npm run build
Then start it in production mode:

npm run start:prod
Additional Commands
Linting:

npm run lint
Cleaning up:

npm run clean
Contributing
Fork this repository and submit pull requests for any improvements or bug fixes.

License
This project is licensed under the MIT License.
