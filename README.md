# ChazeFashion - Django E-commerce Platform

A modern, feature-rich e-commerce platform built with Django for fashion retail. ChazeFashion provides a complete online shopping experience with user authentication, product catalog, shopping cart, wishlist, and order management.

## 🛍️ Features

### Core E-commerce Features
- **Product Catalog**: Browse products with detailed information
- **Advanced Filtering**: Filter by category, season, fabric, price range, and brand
- **Shopping Cart**: Add/remove items, update quantities
- **Wishlist**: Save favorite products for later
- **User Authentication**: Secure signup, login, and logout
- **User Profiles**: Manage personal information and avatar
- **Order Management**: Track order status and history
- **Product Reviews**: Rate and review products
- **Payment Integration**: Support for multiple payment methods

### Product Categories
- Boys
- Girls
- Men
- Women
- Toddler

### Product Attributes
- Name, price, and description
- Category and season classification
- Fabric type and texture
- Brand information
- Stock quantity tracking
- Product images
- Dimensions and weight
- Special offers

## 🚀 Technology Stack

- **Backend**: Django 5.2.4
- **Frontend**: HTML, CSS, JavaScript
- **Styling**: Tailwind CSS (via django-tailwind)
- **Database**: SQLite (development)
- **Image Handling**: Pillow
- **Authentication**: Django's built-in auth system

## 📋 Prerequisites

- Python 3.8 or higher
- pip (Python package installer)
- Git

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd ProductCatlog-master/ChazeFashion
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   ```

3. **Activate the virtual environment**
   - Windows:
     ```bash
     venv\Scripts\activate
     ```
   - macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

5. **Run database migrations**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

6. **Create a superuser (optional)**
   ```bash
   python manage.py createsuperuser
   ```

7. **Run the development server**
   ```bash
   python manage.py runserver
   ```

8. **Access the application**
   Open your browser and navigate to `http://127.0.0.1:8000/`

## 📁 Project Structure

```
ChazeFashion/
├── catalog/                 # Main app for e-commerce functionality
│   ├── models.py           # Database models
│   ├── views.py            # View functions
│   ├── urls.py             # URL routing
│   ├── forms.py            # Form definitions
│   ├── admin.py            # Django admin configuration
│   └── migrations/         # Database migrations
├── ChazeFashion/           # Project settings
│   ├── settings.py         # Django settings
│   ├── urls.py             # Main URL configuration
│   └── wsgi.py             # WSGI configuration
├── templates/              # HTML templates
│   ├── base.html           # Base template
│   └── catalog/            # App-specific templates
├── media/                  # User-uploaded files
├── theme/                  # Tailwind CSS theme
└── manage.py               # Django management script
```

## 🎯 Key Models

### Product
- Product information (name, price, category, etc.)
- Stock management
- Image handling
- Seasonal classification

### UserProfile
- Extended user information
- Avatar upload
- Wallet balance
- Address management

### Cart & CartItem
- Shopping cart functionality
- Quantity management
- User-specific carts

### Wishlist
- User wishlist management
- Product saving functionality

### Order & OrderedItem
- Order processing
- Order history
- Status tracking

### Review
- Product reviews and ratings
- User feedback system

## 🔧 Configuration

### Environment Variables
The project uses Django's default settings. For production, consider setting:

- `SECRET_KEY`: Change the default secret key
- `DEBUG`: Set to `False` in production
- `ALLOWED_HOSTS`: Configure allowed hosts
- `DATABASE_URL`: Configure production database

### Static Files
Static files are served through Django's development server. For production, configure a proper static file server.

## 🚀 Usage

### For Customers
1. **Browse Products**: Visit the home page to see featured products
2. **Search & Filter**: Use the product list page to filter by various criteria
3. **Add to Cart**: Click "Add to Cart" on any product
4. **Manage Cart**: View cart, update quantities, or remove items
5. **Wishlist**: Save products to your wishlist for later
6. **Checkout**: Complete the purchase process

### For Administrators
1. **Django Admin**: Access `/admin/` to manage products, users, and orders
2. **Product Management**: Add, edit, or remove products
3. **Order Management**: Track and update order status
4. **User Management**: Monitor user accounts and profiles

## 🧪 Testing

Run the test suite:
```bash
python manage.py test
```

## 📦 Deployment

### Production Checklist
- [ ] Set `DEBUG = False`
- [ ] Configure production database
- [ ] Set up static file serving
- [ ] Configure media file storage
- [ ] Set secure `SECRET_KEY`
- [ ] Configure `ALLOWED_HOSTS`
- [ ] Set up HTTPS
- [ ] Configure logging
- [ ] Set up monitoring

### Recommended Deployment Options
- **Heroku**: Easy deployment with PostgreSQL
- **DigitalOcean**: VPS with Nginx and Gunicorn
- **AWS**: Elastic Beanstalk or EC2
- **Docker**: Containerized deployment

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🆘 Support

For support and questions:
- Create an issue in the repository
- Contact the development team
- Check the Django documentation

## 🔄 Version History

- **v1.0.0**: Initial release with core e-commerce features
- Basic product catalog and shopping cart functionality
- User authentication and profiles
- Wishlist and order management

---

**Note**: This is a development version. For production use, ensure proper security configurations and testing.
