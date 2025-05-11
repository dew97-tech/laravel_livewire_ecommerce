# Laravel eCommerce Platform

A robust and scalable eCommerce platform built with **Laravel**, **Livewire**, and **Filament**. This project provides a modern, feature-rich online store with a dynamic frontend powered by Livewire and an intuitive admin panel managed via Filament. It supports product management, user authentication, cart functionality, and order processing, making it suitable for small to medium-sized businesses.

## Features

- **Dynamic Frontend**: Interactive UI with Laravel Livewire for real-time updates without page reloads.
- **Admin Dashboard**: Filament-powered admin panel for managing products, orders, users, and categories.
- **Product Management**: Create, update, and delete products with support for images, descriptions, and pricing.
- **Shopping Cart**: Add/remove items, view cart, and proceed to checkout.
- **Order Processing**: Track orders with status updates and user notifications.
- **User Authentication**: Secure registration, login, and role-based access control.
- **Database Support**: Configurable for SQLite or MySQL databases.
- **Responsive Design**: Mobile-friendly interface for seamless user experience.

## Tech Stack

- **Framework**: Laravel 11
- **Frontend**: Livewire 3, Tailwind CSS
- **Admin Panel**: FilamentPHP 3
- **Database**: SQLite (default) or MySQL
- **Server**: PHP 8.2+, Composer
- **Environment**: Laragon (recommended for local development)

## Prerequisites

Before setting up the project, ensure you have the following installed:

- PHP >= 8.2
- Composer
- Node.js and npm
- SQLite or MySQL (based on your `.env` configuration)
- Laragon (optional, for local development)

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```

2. **Install Dependencies**
   ```bash
   composer install
   npm install
   ```

3. **Configure Environment**
   - Copy the `.env.example` file to `.env`:
     ```bash
     cp .env.example .env
     ```
   - Update `.env` with your database settings (SQLite or MySQL):
     ```env
     DB_CONNECTION=sqlite
     DB_DATABASE=/absolute/path/to/database.sqlite
     ```
     or
     ```env
     DB_CONNECTION=mysql
     DB_HOST=127.0.0.1
     DB_PORT=3306
     DB_DATABASE=your_database
     DB_USERNAME=your_username
     DB_PASSWORD=your_password
     ```

4. **Generate Application Key**
   ```bash
   php artisan key:generate
   ```

5. **Run Migrations**
   - Create the database schema:
     ```bash
     php artisan migrate
     ```
   - Optionally, seed the database with sample data:
     ```bash
     php artisan db:seed
     ```

6. **Compile Assets**
   ```bash
   npm run dev
   ```

7. **Start the Server**
   - Using Laravel Artisan:
     ```bash
     php artisan serve
     ```
   - Or use Laragon for a local server setup.

8. **Access the Application**
   - Frontend: `http://localhost:8000`
   - Admin Panel: `http://localhost:8000/admin` (requires admin credentials)

## Usage

- **Admin Access**: Register an admin user via the Filament panel or seed the database with an admin account.
- **Frontend**: Browse products, add to cart, and complete purchases as a guest or registered user.
- **Customization**: Extend the Livewire components or Filament resources in `app/Filament` to add features.

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature/your-feature`.
3. Commit your changes: `git commit -m "Add your feature"`.
4. Push to the branch: `git push origin feature/your-feature`.
5. Open a pull request with a clear description of your changes.

Please adhere to the [Code of Conduct](CODE_OF_CONDUCT.md) and ensure your code follows Laravel coding standards.

## Testing

Run the test suite to ensure the application works as expected:
```bash
php artisan test
```

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- [Laravel](https://laravel.com) for the robust PHP framework.
- [Livewire](https://livewire.laravel.com) for dynamic frontend components.
- [FilamentPHP](https://filamentphp.com) for the powerful admin panel.
- [Laragon](https://laragon.org) for a seamless local development environment.

## Contact

For questions or support, please open an issue or contact [your-email@example.com](mailto:your-email@example.com).

---

Happy selling! 🚀