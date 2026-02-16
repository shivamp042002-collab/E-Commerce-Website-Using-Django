# 🛍️ Bazario – Django E-Commerce Store

Bazario is a modern and responsive E-Commerce web application built using Django and Bootstrap 5.  
It allows users to browse products, view details, add items to cart, and manage products through the Django admin panel.

---

## 🚀 Features

- User Authentication (Login / Register / Logout)
- Product Listing with Categories
- Product Detail Page
- Add to Cart System
- Wishlist Feature
- Admin Dashboard
- Product Image Upload Support
- Responsive Professional UI
- Hero Section with Background Image

---

## 🛠️ Tech Stack

- Backend: Django (Python)
- Frontend: HTML, CSS, Bootstrap 5
- Database: SQLite
- Version Control: Git & GitHub

---

## 📂 Project Setup Guide

### 1️⃣ Clone the Repository

git clone https://github.com/YOUR_USERNAME/bazario.git  
cd bazario  

---

### 2️⃣ Create Virtual Environment

Windows:
python -m venv venv  
venv\Scripts\activate  

Mac/Linux:
python3 -m venv venv  
source venv/bin/activate  

---

### 3️⃣ Install Required Packages

pip install django pillow  

---

### 4️⃣ Apply Migrations

python manage.py makemigrations  
python manage.py migrate  

---

### 5️⃣ Create Superuser (Admin)

python manage.py createsuperuser  

---

### 6️⃣ Run Development Server

python manage.py runserver  

Open in browser:  
http://127.0.0.1:8000/

---

## 🖼️ Media Configuration (Important)

In settings.py add:

MEDIA_URL = '/media/'  
MEDIA_ROOT = os.path.join(BASE_DIR, 'media')  

In main urls.py add:

from django.conf import settings  
from django.conf.urls.static import static  

urlpatterns = [  
    path('', include('store.urls')),  
] + static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)  

---

## 📦 Future Improvements

- Live Search Feature
- Payment Gateway Integration
- Order Management System
- Product Ratings & Reviews
- Dark Mode
- Advanced Admin Dashboard

---

## 👨‍💻 Author

Shivam Pandey  
GitHub: https://github.com/YOUR_USERNAME  

---

## 📜 License

This project is created for educational and portfolio purposes.
