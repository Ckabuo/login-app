# StackUp Backend ExpressJS Part II

Welcome to the login-app project, inspired by StackUp Backend ExpressJS part II campaign! This README provides step-by-step instructions on how to set up and run the project after cloning or downloading it from the GitHub repository.

## Table of Contents
1. [Prerequisites](#prerequisites)
2. [Installation](#installation)
3. [Environment Variables](#environment-variables)
4. [Running the Server](#running-the-server)
5. [Project Structure](#project-structure)
6. [Troubleshooting](#troubleshooting)

## Prerequisites

Before you begin, ensure you have met the following requirements:
- You have installed Node.js and npm. You can download them from [Node.js](https://nodejs.org/).
- You have a MongoDB Atlas account. You can sign up for free at [MongoDB Atlas](https://www.mongodb.com/cloud/atlas).

## Installation

Follow these steps to get your development environment set up:

1. **Clone the repository**:
   ```sh
   git clone https://github.com/your-username/StackUp-BackEnd-ExpressJS-Part-II.git
   cd StackUp-BackEnd-ExpressJS-Part-II
   ```

2. **Navigate to the project directory**:
   ```sh
   cd login-app
   ```

3. **Install the dependencies**:
   ```sh
   npm install
   ```

## Environment Variables

You need to set up your environment variables to connect to your MongoDB database and configure other settings.

1. **Create a `.env` file in the root of the project directory**:
   ```sh
   touch .env
   ```

2. **Add the following variables to your `.env` file**:
   ```sh
   db_connection="your_mongodb_connection_string"
   PORT=3001
   SESSION_SECRET='your_session_secret'
   ```

Replace `your_mongodb_connection_string` with the connection string from your MongoDB Atlas account, and `your_session_secret` with a secret string for your session.

## Running the Server

1. **Start the server**:
   ```sh
   node app.js
   ```

2. **Access the application**:
   - Open your browser and go to `http://localhost:3001`.

## Project Structure

Here is an overview of the project's structure:

```
StackUp-BackEnd-ExpressJS-Part-II/
├── login-app/
│   ├── models/
│   │   └── UserModel.js
│   ├── public/
│   │   └── styles.css
│   ├── views/
│   │   ├── dashboard.ejs
│   │   ├── login.ejs
│   │   ├── register.ejs
│   │   └── welcome.ejs
│   ├── .env
│   ├── app.js
│   ├── package.json
│   └── package-lock.json
```

## Troubleshooting

1. **Common Issues**:
   - Ensure MongoDB connection string is correct and your IP is whitelisted in MongoDB Atlas.
   - Verify that Node.js and npm are installed correctly.
   - Check the environment variables in the `.env` file for any missing or incorrect values.

2. **Debugging**:
   - Use `console.log` statements to debug issues.
   - Check the terminal for server logs and errors.
   - Ensure all dependencies are installed correctly by running `npm install`.

3. **Database Connection Issues**:
   - Make sure your MongoDB Atlas cluster is running.
   - Check if your database credentials in the `.env` file are correct.

If you encounter any issues or have any questions, feel free to open an issue on the GitHub repository. Happy coding!