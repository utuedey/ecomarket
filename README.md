# EcoMarket - An online Marketplace

EcoMarket is a sustainable online marketplace built using Django. 
It aims to provide a platform for eco-conscious buyers and sellers to connect, trade, 
and promote sustainable and environmentally friendly products. 
This README provides an overview of the project and instructions for setting up and running EcoMarket locally.

## Table of Contents
- Features
- Requirements
- Installation
- Configuration
- Usage
- Contributing
- License

## Features
- User authentication and profile management.
- Product listings with detailed descriptions and images.
- Categories and tags for easy product discovery.
- Shopping cart functionality.
- Secure payment processing.
- User reviews and ratings for products.
- Seller profiles and stores.
- Admin dashboard for managing users, products, and orders.

## Requirements
Before you begin, ensure you have met the following requirements:

-Python 3.7+
-Django 3.2+
-Dependencies listed in the `requirements.txt` file

## Installation
1. Clone the EcoMarket repository
```
git clone https://github.com/utuedey/ecomarket.git
```
2. Navigate to the project directory:
```
cd ecomarket
```
3. Create a virual environment(optional but recommended)
```
python -m venv venv
```
4. Activate the virtual environment:
- On Windows:
```
venv\Scripts\activate
```
- On macOS and Linux:
```
source venv/bin/activate
```
5. Install project dependencies:
```
pip install -r requirements.txt
```

## Configuration

1.Create a SQL database for the project.

2.Configure the database settings in the ecomarket/settings.py file. 
Update the DATABASES section with your database information.

3.Create a .env file in the project root directory and set 
the following environment variables:

```
SECRET_KEY=your_secret_key
DEBUG=True
EMAIL_HOST=your_email_host
EMAIL_PORT=your_email_port
EMAIL_USE_TLS=True
EMAIL_HOST_USER=your_email_username
EMAIL_HOST_PASSWORD=your_email_password
```

Replace `your_secret_key`, `your_email_host`, `your_email_port`, 
`your_email_username`, and `your_email_password` with your actual values.

4.Run the following Django management commands to set up the database:
```
python manage.py makemigrations
python manage.py migrate
```
## Usage
1.Start the development server:
```
python manage.py runserver
```
2.Access the EcoMarket web application at http://localhost:8000 in 
your web browser.

3.Create a superuser to access the admin dashboard:
```
python manage.py createsuperuser
```

Follow the prompts to set up the superuser account.

4.Log in to the admin dashboard at http://localhost:8000/admin 
to manage users, products, and orders.


## Contributing
We welcome contributions from the community! If you'd like to contribute to EcoMarket, 
please follow our Contribution Guidelines.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

