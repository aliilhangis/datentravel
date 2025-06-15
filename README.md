# Date'n Travel

A modern travel dating platform that helps people connect and explore the world together.

## Features

- User registration and authentication
- Profile creation and management
- Destination browsing and matching
- Real-time messaging system
- Responsive design for all devices

## Requirements

- PHP 7.4 or higher
- MySQL 5.7 or higher
- Web server (Apache/Nginx)
- Composer (for PHP dependencies)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/datentravel.git
cd datentravel
```

2. Create a MySQL database and import the schema:
```bash
mysql -u root -p < config/schema.sql
```

3. Configure the database connection:
   - Open `config/database.php`
   - Update the database credentials:
     ```php
     define('DB_HOST', 'localhost');
     define('DB_USER', 'your_username');
     define('DB_PASS', 'your_password');
     define('DB_NAME', 'datentravel');
     ```

4. Set up your web server:
   - Point your web server's document root to the `public` directory
   - Ensure the web server has write permissions for the `images` directory

5. Create an `images` directory in the project root:
```bash
mkdir images
chmod 777 images
```

## Directory Structure

```
datentravel/
├── config/
│   ├── database.php
│   └── schema.sql
├── css/
│   └── style.css
├── includes/
│   └── auth.php
├── js/
│   └── main.js
├── public/
│   ├── index.php
│   ├── login.php
│   └── register.php
├── images/
└── README.md
```

## Usage

1. Access the website through your web browser
2. Register a new account or login with existing credentials
3. Complete your profile with personal information and preferences
4. Browse destinations and connect with other travelers
5. Start chatting with your matches

## Security

- All passwords are hashed using PHP's password_hash() function
- SQL injection prevention using prepared statements
- XSS protection through proper output escaping
- CSRF protection implemented in forms

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support, please email support@datentravel.com or create an issue in the repository. 