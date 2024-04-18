# My Shop E-Commerce Application

## Description

My Shop is a full-featured e-commerce application built using Blazor and ASP.NET Core. It allows users to browse products, add items to their cart, place orders, and manage their profile. The application also includes an admin panel for managing products, categories, and more.

## Features

- **Product Catalog** - The application provides a comprehensive product catalog with the following features:

  - Browse products by category
  - Search for products by name or description
  - View detailed product information, including images, description, price, and variants
  - Featured products section on the home page

- **Shopping Cart** - Users can easily add products to their shopping cart and manage cart items:

  - Add products to cart from the product details page
  - Update quantities or remove items from the cart
  - View cart summary with total price
  - Store cart items for authenticated users

- **Order Processing** - The order processing system includes:

  - Checkout process with delivery address form
  - Integration with Stripe payment gateway for secure transactions
  - Order confirmation and success page
  - View order history and details for authenticated users

- **User Authentication** - The application includes a user authentication system:

  - User registration with email and password
  - User login with authentication using JWT tokens
  - User profile management, including password change functionality
  - Role-based authorization for admin access

- **Admin Panel** - The admin panel allows administrators to manage the e-commerce store:
  - Manage products (create, update, delete)
  - Manage product categories and visibility
  - Manage product variants and pricing
  - View and manage orders

#### Technology Stack

- Blazor WebAssembly for the client-side UI
- ASP.NET Core for the server-side API
- Entity Framework Core for database access
- SQL Server for data storage
- Stripe for payment processing
- JSON Web Tokens (JWT) for authentication
- Bootstrap for responsive UI styling

## Installation

1. Prerequisites:

   - .NET 6 SDK
   - SQL Server

2. Clone the repository:

   ```
   git clone https://github.com/yourusername/product-ecommerce-app-dotnet-blazor.git
   ```

3. Configure the database connection string in `appsettings.json`:

   ```json
   "ConnectionStrings": {
     "DefaultConnection": "your-connection-string"
   }
   ```

4. Run the database migrations to create the required tables:

   ```
   dotnet ef database update
   ```

5. Configure Stripe payment gateway:

   - Set your Stripe secret key in `appsettings.json`:
     ```json
     "Stripe": {
       "SecretKey": "your-stripe-secret-key"
     }
     ```

6. Build and run the application:

   ```
   dotnet run
   ```

7. Access the application in your browser at `https://localhost:7226`.

## Usage

- Browse products by navigating to different categories or using the search functionality.
- Click on a product to view its details, select variants (if available), and add it to the cart.
- Manage cart items, update quantities, or remove items as needed.
- Proceed to checkout, fill in the delivery address, and complete the payment using a test credit card.
- View order history and details in the user profile section.
- Admins can access the admin panel to manage products, categories, and orders.

Feel free to explore the various features and functionalities of the My Shop e-commerce application!
