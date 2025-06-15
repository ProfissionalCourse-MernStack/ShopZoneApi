# ShopZone API

Welcome to the ShopZone API, a robust backend solution for e-commerce platforms. This API provides essential features for managing products, categories, users, and orders, ensuring a seamless and efficient online shopping experience.

## Folder Structure

```
ShopZoneApi/
├── config/
│   └── db.js
├── controllers/
│   ├── auth.controller.js
│   ├── category.controller.js
│   ├── product.controller.js
│   └── user.controller.js
├── middleWares/
│   ├── auth.jwt.js
│   └── request.validator.js
├── models/
│   ├── category.model.js
│   ├── order.model.js
│   ├── product.model.js
│   └── user.model.js
├── Routes/
│   ├── auth.route.js
│   ├── category.js
│   ├── product.js
│   └── userRoutes.js
├── utils/
│   └── notificationClient.js
├── validators/
│   └── user.validator.js
├── .env
├── .git/
├── package-lock.json
├── package.json
└── server.js
```

## API Endpoints

- `Auth`: Handles user authentication, including registration and login.
- `Category`: Manages the product categories.
- `Product`: Manages the products in the store.
- `User`: Manages user-related operations.

## Setup and Running the Project

To get the ShopZone API running on your local machine, follow these steps:

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd ShopZoneApi
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Set up environment variables**

   Create a `.env` file in the root directory and add the necessary environment variables. For example:

   ```
   DB_URL=your-mongodb-connection-string
   PORT=5000
   ```

4. **Run the server**

   ```bash
   npm start
   npx nodemon server.js
   ```

The server will start on the port specified in your `.env` file, or on the default port if not specified.
