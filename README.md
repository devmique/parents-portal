# Parent's Portal – Fullstack Web App


---

## Setup Instructions

### 1. Requirements
Before setting up the project, make sure you have the following installed on your machine:
- **Node.js** and **npm** (Node Package Manager)
- **MySQL Server** or access to **phpMyAdmin** for managing MySQL databases

At the root(parents-portal folder)on terminal, run this command:

    
    npm install
    
---


### 2. Backend Setup (Server)

Follow these steps to set up the backend:

1. Open the terminal and navigate to the `server` folder:

    ```bash
    cd server
    ```

2. Install all required dependencies by running:

    ```bash
    npm install
    ```

3. Create a `.env` file inside the `server/` folder and add the following environment variables to configure the database and server settings:

    ```env
    DB_HOST=localhost
    DB_USER=root
    DB_PASSWORD=your_mysql_password
    DB_NAME=parents_portal
    JWT_SECRET=your_jwt_secret
    PORT=5000
    ```

    Replace `your_mysql_password` and `your_jwt_secret` with your actual MySQL password and a secret key for JWT authentication.

4. Start the backend server:

    ```bash
    node server.js
    ```

    This will run the backend server on port 5000 (or any port you configured in the `.env` file).

---

### 3. Frontend Setup (Client)

To set up the frontend, follow these steps:

1. Open the terminal and navigate to the `client` folder:

    ```bash
    cd client
    ```

2. Install all the frontend dependencies:

    ```bash
    npm install
    ```

3. Start the React frontend:

    ```bash
    npm start
    ```

    This will start the frontend app and open it in your default web browser.

---

### 4. Database Setup

1. Open **phpMyAdmin** or **MySQL CLI**.
2. **Create a new database** for the project:

    ```sql
    CREATE DATABASE parents_portal;
    ```

3. **Import the database structure and sample data** from the provided `parents_portal.sql` file. This can be done using the **Import** tab in phpMyAdmin or by running the following command in MySQL CLI:

    ```bash
    mysql -u root -p parents_portal < parents_portal.sql
    ```

    Replace `root` with your MySQL username if it's different.

---

## Author

Made by **Mique Johnlord** 

---





