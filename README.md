# Coffee Blend - Premium Coffee Shop Platform

A full-featured PHP-based coffee shop management platform with online ordering, table booking, and comprehensive admin dashboard.

![PHP](https://img.shields.io/badge/PHP-8.1-blue)
![MySQL](https://img.shields.io/badge/MySQL-10.4-orange)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5.x-purple)
![License](https://img.shields.io/badge/License-MIT-green)

## Features

### Customer Features
- 🛒 **Online Ordering** - Browse and order coffee, drinks, and desserts
- 📅 **Table Booking** - Reserve tables online with date and time selection
- ⭐ **Product Reviews** - View and write reviews for products
- 👤 **User Authentication** - Secure registration and login system
- 🛒 **Shopping Cart** - Add products to cart and manage quantities

### Admin Features
- 📊 **Dashboard** - Overview of orders, bookings, and products
- 🏪 **Product Management** - Create, view, and delete products
- 📝 **Order Management** - View and update order status
- 📅 **Booking Management** - View and manage table reservations
- 👥 **Admin Management** - Create and manage admin accounts

## Technologies Used

- **Backend**: PHP 8.1
- **Database**: MySQL / MariaDB
- **Frontend**: HTML5, CSS3, JavaScript
- **Framework**: Bootstrap 5
- **Database Access**: PDO (PHP Data Objects)
- **Authentication**: bcrypt password hashing

## Installation

### Prerequisites
- PHP 8.1 or higher
- MySQL 10.4 or higher
- Apache/Nginx web server
- Composer (optional)

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/aliaybx/coffee-shop-platform.git
   cd coffee-shop-platform
   ```

2. **Setup Database**
   - Open phpMyAdmin or MySQL CLI
   - Create a new database named `coffee-blend`
   - Import the SQL file:
   ```bash
   mysql -u root -p coffee-blend < SQL_FILE/coffee-blend.sql
   ```

3. **Configure Database Connection**
   Edit `config/config.php`:
   ```php
   define("HOST", "localhost");
   define("DBNAME", "coffee-blend");
   define("USER", "root");
   define("PASS", "your_password");
   ```

4. **Start Local Server**
   Using PHP's built-in server:
   ```bash
   php -S localhost:8000
   ```

5. **Access the Application**
   - Customer Portal: `http://localhost:8000`
   - Admin Panel: `http://localhost:8000/admin-panel`

### Default Admin Credentials
- Email: `admin.first@gmail.com`
- Password: `admin123`

## Project Structure

```
coffee-shop-platform/
├── admin-panel/          # Admin dashboard
│   ├── admins/          # Admin management
│   ├── bookings-admins/ # Booking management
│   ├── orders-admins/   # Order management
│   ├── products-admins/ # Product management
│   ├── layouts/         # Admin layouts
│   └── styles/          # Admin styles
├── auth/                # Authentication
│   ├── login.php        # User login
│   ├── register.php     # User registration
│   └── logout.php       # User logout
├── booking/             # Table booking
├── config/              # Database configuration
├── css/                 # Stylesheets
├── images/              # Image assets
├── includes/            # Reusable PHP includes
├── js/                  # JavaScript files
├── products/            # Product pages
├── reviews/             # Review system
├── SQL_FILE/            # Database SQL
├── users/               # User dashboard
├── index.php            # Homepage
├── menu.php             # Menu page
├── about.php            # About page
├── contact.php          # Contact page
└── services.php         # Services page
```

## Screenshots

### Customer Interface
- Homepage with slider and featured products
- Full menu with categories (drinks, desserts)
- Shopping cart functionality
- Table booking form
- User authentication

### Admin Dashboard
- Product management (CRUD operations)
- Order tracking and status updates
- Booking management
- Admin user creation

## Future Improvements

- [ ] Implement payment gateway integration (Stripe/PayPal)
- [ ] Add email notifications for orders and bookings
- [ ] Implement real-time order status updates
- [ ] Add product categories and filtering
- [ ] Implement multi-language support
- [ ] Add responsive mobile app (React Native/Flutter)
- [ ] Implement order tracking system
- [ ] Add loyalty points and rewards system

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Author

**Ali Ayoub**
- GitHub: [@aliaybx](https://github.com/aliaybx)

## Acknowledgments

- Bootstrap team for the amazing CSS framework
- Colorlib for the original template design
- All contributors who have helped improve this project
