# Inventory Managment

This project is designed to streamline inventory management processes, leveraging the Laravel framework for a robust and scalable solution. It employs MySQL as the database for data persistence and adheres to a Model-View-Controller (MVC) architecture for organized code structure. Additionally, it empowers API integration through well-defined endpoints, enhancing flexibility.

Technologies and Languages:

PHP: The server-side scripting language that powers the application's core functionality.
Laravel: A popular PHP framework providing a structured and efficient foundation for web development.
MySQL: A widely used relational database management system for storing and retrieving inventory data.
CSS: Cascading Style Sheets for defining the visual appearance of the application's user interface.
Blade: Laravel's templating engine, facilitating the creation of dynamic and reusable user interface components.
TypeScript: A superset of JavaScript that adds optional static typing for improved code maintainability and developer experience (consider including it if your project benefits from its features).

# Running the Application

1. **Prerequisites:** Ensure you have PHP and Composer installed on your development system.

2. **Database Setup:**

Create a MySQL database for your inventory management system.
Configure the database connection details in Laravel's .env file.

3. **Migrations:**

Execute the following command to create the database tables based on your models' structure:

Now can run this aplicacion using 

```powershell
    php artisan migrate
```

# Project Structure:

Laravel provides a well-organized directory structure for managing your application's components. Key directories include:

**app:** Contains the core application logic, including models, controllers, and services.
**config:** Houses configuration files for various aspects of the application, such as database connections and application settings.
**public:** Serves as the document root, containing public assets like CSS, JavaScript, and images.
**resources:** Holds views (Blade templates), language files, and other resources.
**routes:** Defines routes for mapping URLs to controller actions.
**tests:** Encompasses unit and integration tests to ensure code quality and functionality.






Plans
    - Generate models
    - Generate controllers
    - Add endpoints by API RESTFULL
    - Design page in Figma

For develop this project, implement this models

    User(name, email, password, transactions)
        Supplier(name, contact, products)
        Administrator(permissions)
        Consumer()
    Product(name, description, price, category, supplier)
    Category(name, description)
    Transaction(timestamp, type, quantity, user, product)
    Location(name, address)
    InventoryLog(Products, location, quantity, date)
    Order(date, status, user) 
    OrderItem(order, product, quantity, price)
