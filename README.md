# Signup Form Project

This is a simple Signup Form web application that allows users to register with their details. It performs both client-side and server-side validation and stores the data in a MySQL database.


# Features

- User-friendly Signup Form
- jQuery-based frontend validations:
  - Required fields
  - Valid email format
  - Valid 10-digit mobile number
  - Strong password check
  - Password confirmation
- PHP backend validation
- Passwords are hashed before saving
- Data stored in MySQL using phpMyAdmin
  

# Technologies Used

- HTML
- jQuery
- PHP
- MySQL (via phpMyAdmin)
- XAMPP (for local server)


## How to Run Locally

1. Start **Apache** and **MySQL** using XAMPP Control Panel.

2. Place this folder inside:  
   **C:\xampp\htdocs\signup_form`**

3. Create a database in 'phpMyAdmin':
   - Name: 'signup_db'
   - Run this SQL to create the table:
     ```sql
     CREATE TABLE users (
       id INT(11) PRIMARY KEY,
       name VARCHAR(100) NOT NULL,
       email VARCHAR(100) NOT NULL UNIQUE,
       mobile int10) NOT NULL,
       password VARCHAR(255) NOT NULL,
       created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
     );
     ```
4. Open your browser and go to:  
   **http://localhost/signup_form/signup.html**
   
5. Fill the form and click **Signup**.
   
6. Now go to: **http://localhost/phpmyadmin**

7. Data will be stored in the `users` table.
