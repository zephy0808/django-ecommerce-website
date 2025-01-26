# Django eCommerce Website

This project is a full-fledged eCommerce website built using Django, a high-level Python web framework. It includes essential features such as user authentication, product browsing, cart management, checkout process, payment integration, and more. The website is designed to be robust, scalable, and user-friendly, providing a seamless shopping experience for customers.

## Table of Contents

- [Features](#features)
- [Screenshots](#screenshots)
- [Technologies Used](#technologies-used)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

- **User Authentication:** Secure user registration, login, reset password, and profile management.
- **Product Catalog:** Browse and search products with detailed descriptions and images.
- **Shopping Cart:** Add, update, and remove items from the cart seamlessly.
- **Checkout Process:** Smooth checkout flow with order summary and address management.
- **Payment Integration:** Integrated with Razorpay for secure online payments.
- **Order Management:** View order history and status updates.
- **Responsive Design:** Mobile-friendly UI ensuring a consistent experience across devices.
- **Admin Panel:** Manage products, orders, and users efficiently through Django's admin interface.

## Screenshots

### Home Page

![Homepage Screenshot](Screenshots/Home-Django-Ecommerce-Site.png)

### Wishlist Page

![Wishlist Screenshot](Screenshots/Wishlist.png)

### Order History Page

![Order-History Screenshot](Screenshots/Order-History.png)

### Order Details Page

![Order-Deatils Screenshot](Screenshots/Order-Details.png)

### Contact-Us Page

![Contact-Us Screenshot](Screenshots/Contact-Us.png)

### About-Us Page

![About-Us Screenshot](Screenshots/About-Us.png)

### Product Page

![Product Page Screenshot](Screenshots/Product-Image.png)

### Shopping Cart Page

![Cart Page Screenshot](Screenshots/Shopping-Cart.png)

### Payment Testing View Page

![Payment Testing Page Screenshot](Screenshots/Payment-Testing-View.png)

### Payment Success Page

![Payment Success Page Screenshot](Screenshots/Payment-Successful.png)

### Login Page

![Login Page Screenshot](Screenshots/Login.png)

### Register Page

![Register Page Screenshot](Screenshots/Register.png)

### Reset Password Page

![Reset Password Page Screenshot](Screenshots/Password-Reset-Form.png)

### Profile Page

![Profile Page Screenshot](Screenshots/Profile.png)

### Shipping Address Page

![Shipping Address Page Screenshot](Screenshots/Shipping-Address.png)

### Change Password View

![Change Password Page Screenshot](Screenshots/Change-Password-Page.png)

## Technologies Used

- **Django:** Python-based web framework for backend development.
- **HTML/CSS/JavaScript:** Frontend development for a responsive and interactive UI.
- **Razorpay API:** Payment gateway integration for secure transactions.
- **Bootstrap:** Frontend framework for responsive design and UI components.

## Setup Instructions

To run this project locally, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/atulguptag/Django-eCommerce-Website.git
   cd Django-eCommerce-Website
   ```

2. **Create a virtual environment:**
   ```bash
   python -m venv venv
   ```
3. **Activate the virtual environment:**

   - On Windows:
     ```bash
     .\venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

### `Note: If you face any kind of issue while installing the packages or by running the above command, you can follow this step - `

- First, run the below pip command into your terminal (make sure your virtual environment is activated, it should be something like that - `(venv) PS C:\Users\asus\Django-eCommerce-Website`)-

  ```bash
  pip install django python-decouple django-allauth django_countries django-crispy-forms crispy_bootstrap4 jwt
  ```

- and so on...

- Second, you should create `.env` file in your project root, and update it with the same as `.env.example`

- Then, you should add `SECRET_KEY` and `DEBUG=True` in `.env` file -

- **How to generate/get the SECRET_KEY?**

- Follow this step - Open your terminal in VS Code, then type `django-admin shell`, and hit enter.

- Paste the below code into your shell -

  ```bash
  from django.core.management.utils import get_random_secret_key
  get_random_secret_key()
  ```

* Copy the `SECRET_KEY`(whatever you got in the output), and paste it in your `.env` file.

* Now, install as many packages as you want to use, then follow the next steps -

5. **Apply database migrations:**

   ```bash
   python manage.py migrate
   ```

6. **Create a superuser (admin):**

   ```bash
   python manage.py createsuperuser
   ```

7. **Start the development server:**

   ```bash
   python manage.py runserver
   ```

8. **Open your web browser and navigate to:**
   ```
   http://127.0.0.1:8000/
   ```

## Usage

- **Admin Panel:** Access the admin panel at `http://127.0.0.1:8000/admin/` to manage products, orders, and users.
- **Shopping:** Browse products, add items to the cart, proceed to checkout, and make payments using Razorpay.
- **Profile:** Users can register, login, reset their password, view their order history, and update their profiles.

## Contributing

Contributions are welcome! Please fork this repository and create a pull request with your proposed features, enhancements, or bug fixes.

## License

This project is licensed under the [MIT License](LICENSE).
