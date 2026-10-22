 # Inventory Management REST API

A RESTful API for managing inventory products using Node.js, Express.js, and MongoDB. This project supports CRUD operations to create, retrieve, update, and delete product records.

## Project Description

The Inventory Management REST API helps manage product information, including product name, price, quantity, and category. It uses MongoDB to store product data and provides REST API endpoints that can be tested using Postman.

## Features

- Create a new product
- Retrieve all products
- Retrieve a single product by ID
- Update product information
- Delete a product
- Store product data in MongoDB Atlas
- Test API endpoints using Postman

## Technologies Used

- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- JavaScript
- Postman
- Git and GitHub

## Project Structure

```text
Inventory-REST-API/
├── config/
│   └── db.js
├── controllers/
│   └── productController.js
├── models/
│   └── product.js
├── routes/
│   └── productRoutes.js
├── .gitignore
├── app.js
├── package.json
├── package-lock.json
└── README.md
```

## API Endpoints

Base URL: `http://localhost:5000`

| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/products` | Get all products |
| GET | `/api/products/:id` | Get a product by ID |
| POST | `/api/products` | Create a new product |
| PUT | `/api/products/:id` | Update a product |
| DELETE | `/api/products/:id` | Delete a product |

## Sample Product JSON

Use this JSON body when creating or updating a product in Postman:

```json
{
	"name": "Laptop",
	"price": 55000,
	"quantity": 10,
	"category": "Electronics"
}
```

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/jaymaskare0715/Inventory-REST-API.git
```

### 2. Navigate to the Project Folder

```bash
cd Inventory-REST-API
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Configure Environment Variables

Create a `.env` file in the project root folder and add:

```env
PORT=5000
MONGO_URI=your_mongodb_atlas_connection_string
```

Replace the placeholder with your MongoDB Atlas connection string. Never commit your `.env` file or publish database credentials.

### 5. Start the Server

For development:

```bash
npm run dev
```

Or run:

```bash
npm start
```

The API will run at:

`http://localhost:5000`

## Testing with Postman

1. Start the API server.
2. Open Postman.
3. Send requests to `http://localhost:5000/api/products`.
4. Select the appropriate HTTP method.
5. For POST and PUT, choose **Body → raw → JSON** and provide the product data.
6. Check the response and HTTP status code.

## Learning Outcomes

- Understanding REST API development
- Implementing CRUD operations
- Connecting Node.js applications to MongoDB Atlas
- Organizing code using models, controllers, and routes
- Testing APIs using Postman
- Managing source code with Git and GitHub

## Author

**Jay Santosh Maskare**

GitHub: [@jaymaskare0715](https://github.com/jaymaskare0715)
