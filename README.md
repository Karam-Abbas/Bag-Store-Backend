# Online Bag Store (Backend Project)

## Overview

This is an Express.js application designed to manage users, products, and owners. The application is structured using a Model-View-Controller (MVC) pattern and includes the following features:

- User management
- Product management
- Owner management
- Flash messaging
- Session handling

## Features

- **User Management:** Create, read, update, and delete users.
- **Product Management:** Create, read, update, and delete products.
- **Owner Management:** Create, read, update, and delete owners.
- **Session Management:** Maintain user sessions.
- **Flash Messaging:** Display flash messages for various operations.

## Prerequisites

- Node.js (v14 or higher recommended)
- npm (v6 or higher recommended)
- MongoDB

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/your-repo-name.git
    cd your-repo-name
    ```

2. Install dependencies:

    ```bash
    npm install
    ```

3. Create a `.env` file in the root directory and add your environment variables:

    ```env
    PORT=3000
    DB_URI=mongodb://localhost:27017/your-database-name
    SESSION_SECRET=your-session-secret
    ```

4. Start the MongoDB server (if not already running):

    ```bash
    mongodb
    ```

5. Start the application:

    ```bash
    npm start
    ```

    The application should now be running at `http://localhost:3000`.

## Project Structure

```
.
├── config
│   └── mongoose-connection.js   # MongoDB connection setup
├── public                       # Static files (CSS, JS, images)
├── routes
│   ├── index.js                 # Index route
│   ├── ownersRouter.js          # Owner routes
│   ├── productsRouter.js        # Product routes
│   └── usersRouter.js           # User routes
├── views                        # EJS templates
├── .env                         # Environment variables
├── app.js                       # Main application file
└── package.json                 # Project metadata and dependencies
```

## Usage

- **Home:** Visit `http://localhost:3000` to access the home page.
- **Users:** Visit `http://localhost:3000/users` to manage users.
- **Owners:** Visit `http://localhost:3000/owners` to manage owners.
- **Products:** Visit `http://localhost:3000/products` to manage products.

## Dependencies

- [bcrypt](https://www.npmjs.com/package/bcrypt) - Library to help hash passwords
- [config](https://www.npmjs.com/package/config) - Node.js application configuration
- [connect-flash](https://www.npmjs.com/package/connect-flash) - Flash message middleware for Express
- [cookie-parser](https://www.npmjs.com/package/cookie-parser) - Parse cookies
- [debug](https://www.npmjs.com/package/debug) - Tiny debugging utility
- [dotenv](https://www.npmjs.com/package/dotenv) - Loads environment variables from a `.env` file
- [ejs](https://www.npmjs.com/package/ejs) - Embedded JavaScript templates
- [express](https://www.npmjs.com/package/express) - Web framework for Node.js
- [express-session](https://www.npmjs.com/package/express-session) - Session middleware for Express
- [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken) - JSON Web Token implementation
- [mongoose](https://www.npmjs.com/package/mongoose) - MongoDB object modeling for Node.js

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/feature-name`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/feature-name`)
5. Open a pull request

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

