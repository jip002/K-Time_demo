# KTime Project Setup Guide

The project consists of a React.js frontend and an Express.js + MySQL backend which for now can be run on local machine.

Please ensure you have Node.js and MySQL installed on your system:
- [Node.js](https://nodejs.org/)
- [MySQL](https://dev.mysql.com/downloads/)

## Database Setup

1. Start your MySQL service.
2. Create a new MySQL database:
   ```sql
   CREATE DATABASE KTimeDB;

## Backend Setup

1. Navigate to the `server` folder and install dependencies:
   ```bash
   cd server
   npm install
2. start the server
   ```bash
   npm start

## Frontend Setup
1. Navigate to the client folder and install dependencies:
    ```bash
    cd client
    npm install
2. Start the React development server:
    ```bash
    npm start

The frontend should now be accessible at http://localhost:3000, and the backend should be serving on http://localhost:3001.

## Configuration
1. Adjust your MySQL configuration as needed in server/config/config.json:
    ```bash
    {
        "development": {
            "username": "root",
            "password": "password",
            "database": "KTimeDB",
            "host": "127.0.0.1",
            "dialect": "mysql"
        }
    }

2. Replace "password" with your actual MySQL root password.