
---

# Login Page with User Authentication

This project demonstrates a login page that allows users to authenticate using their credentials. The login process verifies the username and password against a database, ensuring secure access to a user's profile or dashboard.

## Table of Contents

- [Introduction](#introduction)
- [Technologies Used](#technologies-used)
- [Features](#features)
- [Setup](#setup)
- [Usage](#usage)
- [License](#license)

## Introduction

This login page provides a secure way for users to access protected areas of a web application. It includes frontend validation using HTML and JavaScript, and backend authentication using PHP with MySQL. Passwords are stored securely in the database with hashing for enhanced security.

## Technologies Used

- **Frontend**:
  - HTML (for the login form)
  - CSS (for styling the page)
  - JavaScript (for client-side validation)

- **Backend**:
  - PHP (for handling form submissions and user authentication)
  - MySQL (for storing user data)

- **Tools**:
  - XAMPP or WAMP (local server environment)
  - Git (version control)

## Features

- **Secure Authentication**: Passwords are hashed and verified using PHP's `password_hash()` and `password_verify()` functions.
- **Client-Side Validation**: Ensures that both the username and password fields are filled before submission.
- **Responsive Design**: The login form is styled to be responsive and work on both desktop and mobile devices.
- **Error Handling**: Displays error messages for invalid credentials or failed authentication.

## Setup

Follow these steps to set up the project on your local machine:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/login-page.git
   ```

2. **Set up the database**:
   - Create a MySQL database named `login_app`.
   - Run the provided SQL script (`database.sql`) to create the necessary tables, especially the `users` table with columns for `username` and `password`.

3. **Configure database connection**:
   - Open the `config.php` file and update the database credentials:
     ```php
     $host = 'localhost';
     $user = 'root';
     $pass = '';
     $dbname = 'login_app';
     ```

4. **Start the server**:
   - Use XAMPP or WAMP to start the Apache and MySQL servers.

5. **Access the login page**:
   - Navigate to `http://localhost/login-page` in your web browser.

## Usage

- **Login**: Enter your username and password in the login form. If the credentials are correct, you will be redirected to the dashboard page.
- **Invalid Credentials**: If the username or password is incorrect, an error message will be displayed.
- **Password Hashing**: The application uses PHP's `password_hash()` to securely store and verify passwords.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for more information.

