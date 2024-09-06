# BookHub - Book Purchasing Web Application

Welcome to **BookHub**, an online platform designed to simplify the process of browsing, selecting, and purchasing books. This web application offers a smooth user experience for customers, allowing them to search for books, manage shopping carts, and complete purchases. Additionally, it includes an admin panel for managing books and orders.

## Features

### User Features
- **Book Catalog**: Explore a wide range of books with detailed descriptions, prices, and cover images.
- **Search Functionality**: Easily find books by title, author, or genre using the search bar.
- **Shopping Cart**: Add books to your cart, modify quantities, or remove items before checkout.
- **Checkout Process**: Complete purchases through a secure and straightforward checkout process.
- **User Authentication**: Register and log in to access personalized features, such as order history.

### Admin Features
- **Customer Management**: View and manage registered users.
- **Book Management**: Add, edit, or remove books from the inventory.
- **Order Management**: Track and update the status of customer orders.

## File Structure

- **css/**: Contains stylesheets used for designing the user interface.
- **font/css/**: Custom fonts used for consistent typography across the app.
- **image/**: Stores images, including book covers and other visual assets.
- **js/**: JavaScript files that add interactivity and dynamic behavior to the app.
- **uploaded_img/**: Stores user-uploaded images, such as book covers added by the admin.

## Technologies Used
- **Front-end**: HTML, CSS, JavaScript
- **Back-end**: PHP
- **Database**: MySQL
- **Version Control**: Git (for source code management)

## Installation Instructions

### Prerequisites
- A local server environment like **XAMPP** or **WAMP**.
- **PHP** and **MySQL** installed on your machine.

### Setup Steps

1. **Clone the repository**:
   ```bash
   git clone https://github.com/NipunaMadula/BookHub.git

2. **Set up the database**:
   - Import the provided SQL file (usually `db.sql` or `book_store.sql`) into your MySQL database.

3. **Configure the database connection**:
   - Open the `config.php` file and enter your database credentials:
     ```php
     $dbHost = 'localhost';
     $dbUser = 'root';
     $dbPass = 'your_password';
     $dbName = 'book_store';
     ```

4. **Run the application**:
   - Open your browser and go to `http://localhost/BookHub`.

5. **Verify the setup**:
   - Ensure that user registration, login, and book browsing features are working.
   - Test adding books to the cart, checking out, and viewing the order history.

6. **Admin Access**:
   - After registering a user, manually update the role in the MySQL database to grant admin privileges:
     ```sql
     UPDATE users SET role = 'admin' WHERE email = 'admin@example.com';
     ```

## Troubleshooting

If you encounter issues, here are some common solutions:

- **Database connection errors**: Verify that the credentials in `config.php` are correct, and ensure that the MySQL server is running.
- **Permission issues**: Ensure the necessary permissions are set for the `uploaded_img/` directory to allow file uploads.
- **404 Page Not Found**: Ensure your server is pointing to the correct directory (e.g., `htdocs/BookHub` for XAMPP).

## Contributing

We welcome contributions! Follow these steps to contribute to the project:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m "Add new feature"`).
4. Push to your branch (`git push origin feature-branch`).
5. Open a pull request for review.

## Contact

For any questions or suggestions, feel free to reach out:

- **Author**: [Nipuna Madula](https://github.com/NipunaMadula)
- **Email**: nipunamadula2001@gmail.com
