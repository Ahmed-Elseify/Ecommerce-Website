# 🛒 Django E-Commerce Platform

A full-stack e-commerce web application powered by Django. It includes a dynamic storefront catalog, session-based cart management, secure checkout with PayPal payment integration, and administrative authentication using Django's built-in auth and admin interfaces.

## Features

- **Storefront & Catalog**: Dynamic product showcase with category filtering, detailed product pages, and availability tracking.
- **Cart & Order Flow**: Real-time cart updates, quantity management, automated total calculation, and checkout summaries.
- **PayPal Payment Gateway**: Client/server PayPal integration for secure order capture and transaction verification.
- **User Authentication & Management**: Administrative login/logout, staff permissions, and order tracking through Django Auth/Admin.
- **Inventory & Order Administration**: Product, customer order, and transaction status management through Django Admin.

## Tech Stack

- **Backend**: Python, Django
- **Database**: SQLite (development default) / PostgreSQL
- **Frontend**: Django Templates (HTML5, CSS3, JavaScript), Bootstrap or Tailwind CSS
- **Payments**: PayPal REST SDK / PayPal JavaScript SDK

## Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/Ahmed-Elseify/Ecommerce-Website.git
   cd Ecommerce-Website
   ```

2. **Create and activate a virtual environment**

   ```bash
   python -m venv venv
   ```

   - Windows:

     ```bash
     venv\Scripts\activate
     ```

   - macOS/Linux:

     ```bash
     source venv/bin/activate
     ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**

   Create a `.env` file in the project root:

   ```env
   SECRET_KEY=your_django_secret_key
   DEBUG=True
   PAYPAL_CLIENT_ID=your_paypal_sandbox_client_id
   PAYPAL_SECRET=your_paypal_sandbox_secret
   ```

5. **Apply database migrations**

   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

6. **Create an admin superuser**

   ```bash
   python manage.py createsuperuser
   ```

7. **Run the development server**

   ```bash
   python manage.py runserver
   ```
