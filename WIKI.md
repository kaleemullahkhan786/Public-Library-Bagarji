# 📚 Public Library Bagarji - Complete Wiki Documentation

<div align="center">

![Library Logo](https://raw.githubusercontent.com/Public-Library-Bagarji/Media/main/Static_img/websitemainlogo.jpg)

### 🏆 **Complete Technical Documentation & User Guide** 🏆

**Comprehensive Wiki for Developers, Administrators, and End Users**

[![Documentation](https://img.shields.io/badge/Documentation-Wiki-blue.svg)](https://github.com/kaleemullahkhan786/Public-Library-Bagarji/wiki)
[![Version](https://img.shields.io/badge/Version-1.0.0-green.svg)](https://github.com/kaleemullahkhan786/Public-Library-Bagarji)
[![Last Updated](https://img.shields.io/badge/Last%20Updated-July%202025-orange.svg)](https://github.com/kaleemullahkhan786/Public-Library-Bagarji)

</div>

---

## 📋 **Table of Contents**

1. [🚀 Quick Start Guide](#-quick-start-guide)
2. [📖 User Manual](#-user-manual)
3. [⚙️ System Administration](#️-system-administration)
4. [🔧 Developer Guide](#-developer-guide)
5. [🛠️ Technical Documentation](#️-technical-documentation)
6. [🔒 Security Guide](#-security-guide)
7. [📊 Analytics & Monitoring](#-analytics--monitoring)
8. [🚀 Deployment Guide](#-deployment-guide)
9. [❓ FAQ & Troubleshooting](#-faq--troubleshooting)
10. [📞 Support & Contact](#-support--contact)

---

## 🚀 **Quick Start Guide**

### **For End Users**

#### **1. Accessing the Library**
- **URL**: https://publiclibrarybagarji.com
- **Mobile App**: Available on App Store and Google Play
- **Browser Support**: Chrome, Firefox, Safari, Edge

#### **2. Creating an Account**
1. Click "Register" on the homepage
2. Fill in your details (Name, Email, Phone)
3. Verify your email with OTP
4. Complete your profile setup

#### **3. Browsing Books**
1. Navigate to "Books" section
2. Use search bar for specific titles/authors
3. Apply filters by category, availability
4. Click on book for detailed view

#### **4. Reading Books**
1. Select a book from the catalog
2. Choose reading format (PDF, Online Reader)
3. Download or read online
4. Add to your reading list

### **For Administrators**

#### **1. Initial Setup**
```bash
# Clone repository
git clone https://github.com/kaleemullahkhan786/Public-Library-Bagarji.git

# Install dependencies
pip install -r requirements.txt

# Configure environment
cp env.example .env
# Edit .env with your settings

# Run migrations
python manage.py migrate

# Create superuser
python manage.py createsuperuser

# Start server
python manage.py runserver
```

#### **2. Admin Panel Access**
- **URL**: https://yourdomain.com/admin/
- **Username**: Your superuser credentials
- **Features**: Complete content management

---

## 📖 **User Manual**

### **📚 Book Management**

#### **Browsing Books**
- **Search**: Use the search bar for quick book finding
- **Filters**: Filter by category, author, availability
- **Sorting**: Sort by title, date, popularity
- **Pagination**: Navigate through large catalogs

#### **Reading Books**
- **PDF Download**: Download books for offline reading
- **Online Reader**: Read directly in browser
- **Bookmarking**: Save your reading progress
- **Notes**: Add personal notes to books

#### **Book Reviews**
- **Rating System**: Rate books from 1-5 stars
- **Review Writing**: Write detailed reviews
- **Review Reading**: Read other users' reviews
- **Helpful Votes**: Vote on helpful reviews

### **📰 Content Management**

#### **Blogs & Articles**
- **Reading**: Browse educational articles
- **Categories**: Filter by topic categories
- **Search**: Find specific content
- **Sharing**: Share articles on social media

#### **News & Updates**
- **Latest News**: Stay updated with library news
- **Events**: View upcoming events
- **Announcements**: Important announcements
- **Notifications**: Email notifications for updates

### **👥 User Features**

#### **Profile Management**
- **Profile Picture**: Upload and manage profile photos
- **Personal Info**: Update contact information
- **Reading History**: Track your reading progress
- **Favorites**: Save favorite books and articles

#### **Community Features**
- **Comments**: Comment on books and articles
- **Discussions**: Participate in community discussions
- **Recommendations**: Get personalized recommendations
- **Social Features**: Connect with other readers

---

## ⚙️ **System Administration**

### **🔧 Admin Panel Guide**

#### **Dashboard Overview**
- **Analytics**: View site statistics and user activity
- **Quick Actions**: Common administrative tasks
- **System Status**: Monitor system health
- **Recent Activity**: Latest user and content activity

#### **Content Management**

##### **Books Management**
```
Admin Panel → Library Admin → Books
```
- **Add New Book**: Upload books with metadata
- **Edit Books**: Modify book information
- **Delete Books**: Remove books from catalog
- **Bulk Operations**: Manage multiple books

##### **Categories Management**
```
Admin Panel → Library Admin → Categories
```
- **Create Categories**: Organize content
- **Edit Categories**: Modify category details
- **Category Types**: Book, Blog, News categories
- **Category Hierarchy**: Nested categories

##### **Articles & Blogs**
```
Admin Panel → Library Admin → Articles
```
- **Create Articles**: Write educational content
- **Rich Text Editor**: Format content with markdown
- **Image Upload**: Add images to articles
- **SEO Settings**: Optimize for search engines

##### **News Management**
```
Admin Panel → Library Admin → News
```
- **Publish News**: Share library updates
- **News Categories**: Organize news by type
- **Scheduling**: Schedule news publication
- **Featured News**: Highlight important news

#### **User Management**

##### **User Administration**
```
Admin Panel → Public Site → Users
```
- **User List**: View all registered users
- **User Details**: Access user profiles
- **Account Status**: Activate/deactivate accounts
- **User Roles**: Manage user permissions

##### **User Profiles**
```
Admin Panel → Public Site → User Profiles
```
- **Profile Information**: View user details
- **Profile Images**: Manage user photos
- **Contact Information**: Access user contact details
- **Account History**: View user activity

#### **Comment Management**

##### **Comments Overview**
```
Admin Panel → Comments → Blog Comments
Admin Panel → Comments → Book Comments
```
- **Moderate Comments**: Approve/reject comments
- **Reply to Comments**: Admin responses
- **Comment Analytics**: Track engagement
- **Spam Protection**: Filter spam comments

### **📊 Analytics Dashboard**

#### **Site Analytics**
- **Visitor Statistics**: Daily, weekly, monthly visitors
- **Page Views**: Most popular pages
- **User Engagement**: Time spent on site
- **Traffic Sources**: Where visitors come from

#### **Content Analytics**
- **Popular Books**: Most read books
- **Popular Articles**: Most viewed content
- **Search Analytics**: What users search for
- **Download Statistics**: Book download counts

#### **User Analytics**
- **User Registration**: New user signups
- **Active Users**: Daily, weekly active users
- **User Behavior**: How users interact with site
- **Device Analytics**: Mobile vs desktop usage

---

## 🔧 **Developer Guide**

### **🏗️ Project Architecture**

#### **Django Apps Structure**
```
public_library_bagarji/
├── library_admin/          # Main library functionality
│   ├── models.py          # Database models
│   ├── views.py           # View logic
│   ├── admin.py           # Admin interface
│   ├── forms.py           # Form handling
│   └── urls.py            # URL routing
├── public_site/           # User-facing features
│   ├── models.py          # User models
│   ├── views.py           # Public views
│   ├── middleware.py      # Custom middleware
│   └── urls.py            # URL routing
├── comments/              # Comment system
├── library_requests/      # Book request system
├── messages_requests/     # Messaging system
└── public_library_project/ # Main project settings
```

#### **Database Schema**

##### **Core Models**
```python
# Book Management
class Book(models.Model):
    title = models.CharField(max_length=200)
    author = models.CharField(max_length=100)
    description = models.TextField()
    pdf_file = models.FileField(upload_to='book_pdfs/')
    cover_image = models.ImageField(upload_to='book_covers/')
    category = models.ForeignKey(Category, on_delete=models.PROTECT)
    slug = models.SlugField(unique=True)
    available = models.BooleanField(default=True)

# Content Management
class Article(models.Model):
    title = models.CharField(max_length=200)
    content = models.TextField()
    author = models.CharField(max_length=100)
    category = models.ForeignKey(Category, on_delete=models.PROTECT)
    image = models.ImageField(upload_to='blog_images/')
    slug = models.SlugField(unique=True)

# User Management
class UserProfile(models.Model):
    user = models.OneToOneField(User, on_delete=models.CASCADE)
    phone = models.CharField(max_length=20)
    gender = models.CharField(max_length=10, choices=GENDER_CHOICES)
    profile_image = models.ImageField(upload_to='uploads/profiles/')
```

### **🔧 Development Setup**

#### **Environment Setup**
```bash
# Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Install development dependencies
pip install django-debug-toolbar
pip install coverage
pip install black
pip install flake8
```

#### **Database Setup**
```bash
# SQLite (Development)
python manage.py migrate

# PostgreSQL (Production)
# Update settings.py with database configuration
python manage.py migrate
```

#### **Static Files Setup**
```bash
# Collect static files
python manage.py collectstatic

# Serve static files in development
python manage.py runserver
```

### **🧪 Testing Guide**

#### **Running Tests**
```bash
# Run all tests
python manage.py test

# Run specific app tests
python manage.py test library_admin

# Run with coverage
coverage run --source='.' manage.py test
coverage report
coverage html
```

#### **Test Structure**
```
tests/
├── test_models.py         # Model tests
├── test_views.py          # View tests
├── test_forms.py          # Form tests
├── test_admin.py          # Admin tests
└── test_integration.py    # Integration tests
```

### **🔍 Code Quality**

#### **Code Formatting**
```bash
# Format code with Black
black .

# Check code style with flake8
flake8 .

# Sort imports
isort .
```

#### **Pre-commit Hooks**
```bash
# Install pre-commit
pip install pre-commit

# Setup hooks
pre-commit install

# Run hooks manually
pre-commit run --all-files
```

---

## 🛠️ **Technical Documentation**

### **🔧 API Documentation**

#### **REST API Endpoints**

##### **Books API**
```http
GET /api/books/                    # List all books
GET /api/books/{id}/               # Get specific book
POST /api/books/                   # Create new book (Admin)
PUT /api/books/{id}/               # Update book (Admin)
DELETE /api/books/{id}/            # Delete book (Admin)
```

##### **Articles API**
```http
GET /api/articles/                 # List all articles
GET /api/articles/{id}/            # Get specific article
POST /api/articles/                # Create article (Admin)
PUT /api/articles/{id}/            # Update article (Admin)
DELETE /api/articles/{id}/         # Delete article (Admin)
```

##### **Users API**
```http
GET /api/users/                    # List users (Admin)
GET /api/users/{id}/               # Get user profile
POST /api/users/register/          # User registration
POST /api/users/login/             # User login
PUT /api/users/{id}/               # Update profile
```

#### **API Authentication**
```python
# JWT Token Authentication
from rest_framework_simplejwt.tokens import RefreshToken

# Generate tokens
refresh = RefreshToken.for_user(user)
access_token = refresh.access_token
```

### **📊 Database Optimization**

#### **Indexing Strategy**
```sql
-- Book search optimization
CREATE INDEX idx_book_title ON library_admin_book(title);
CREATE INDEX idx_book_author ON library_admin_book(author);
CREATE INDEX idx_book_category ON library_admin_book(category_id);

-- User activity optimization
CREATE INDEX idx_sitevisit_timestamp ON public_site_sitevisit(timestamp);
CREATE INDEX idx_sitevisit_user ON public_site_sitevisit(user_id);
```

#### **Query Optimization**
```python
# Optimized book queries
books = Book.objects.select_related('category').prefetch_related('reviews')

# Optimized user queries
users = User.objects.select_related('userprofile').prefetch_related('groups')
```

### **🎨 Frontend Architecture**

#### **CSS Architecture**
```css
/* Theme System */
:root {
    --fire-primary: #ff3300;
    --fire-secondary: #ff6600;
    --bg-primary: #ffffff;
    --text-primary: #2c3e50;
}

/* Responsive Design */
@media (max-width: 767px) {
    .container { padding: 0 15px; }
    .hero-title { font-size: 2rem; }
}
```

#### **JavaScript Structure**
```javascript
// Main application
class LibraryApp {
    constructor() {
        this.init();
    }
    
    init() {
        this.setupEventListeners();
        this.initializeComponents();
    }
    
    setupEventListeners() {
        // Search functionality
        document.querySelector('.search-input').addEventListener('input', this.handleSearch);
        
        // Theme toggle
        document.querySelector('.theme-toggle').addEventListener('click', this.toggleTheme);
    }
}
```

---

## 🔒 **Security Guide**

### **🛡️ Security Implementation**

#### **Authentication & Authorization**
```python
# User authentication
from django.contrib.auth.decorators import login_required
from django.contrib.auth.mixins import LoginRequiredMixin

# Admin-only views
@login_required
def admin_dashboard(request):
    if not request.user.is_staff:
        return redirect('home')
    return render(request, 'admin/dashboard.html')
```

#### **CSRF Protection**
```python
# CSRF token in forms
{% csrf_token %}

# AJAX CSRF setup
function getCookie(name) {
    let cookieValue = null;
    if (document.cookie && document.cookie !== '') {
        const cookies = document.cookie.split(';');
        for (let i = 0; i < cookies.length; i++) {
            const cookie = cookies[i].trim();
            if (cookie.substring(0, name.length + 1) === (name + '=')) {
                cookieValue = decodeURIComponent(cookie.substring(name.length + 1));
                break;
            }
        }
    }
    return cookieValue;
}

const csrftoken = getCookie('csrftoken');
```

#### **Input Validation**
```python
# Form validation
from django import forms

class BookForm(forms.ModelForm):
    def clean_title(self):
        title = self.cleaned_data['title']
        if len(title) < 3:
            raise forms.ValidationError("Title must be at least 3 characters long.")
        return title
    
    def clean_pdf_file(self):
        pdf_file = self.cleaned_data['pdf_file']
        if pdf_file:
            if pdf_file.size > 50 * 1024 * 1024:  # 50MB limit
                raise forms.ValidationError("PDF file size must be under 50MB.")
        return pdf_file
```

#### **File Upload Security**
```python
# Secure file upload
import os
from django.core.files.storage import FileSystemStorage

class SecureFileStorage(FileSystemStorage):
    def get_valid_name(self, name):
        # Sanitize filename
        name = super().get_valid_name(name)
        # Check file extension
        ext = os.path.splitext(name)[1].lower()
        allowed_extensions = ['.pdf', '.jpg', '.jpeg', '.png']
        if ext not in allowed_extensions:
            raise ValueError(f"File type {ext} not allowed.")
        return name
```

### **🔍 Security Testing**

#### **Automated Security Tests**
```python
# Security test cases
from django.test import TestCase
from django.urls import reverse

class SecurityTestCase(TestCase):
    def test_sql_injection_protection(self):
        # Test SQL injection attempts
        response = self.client.get(reverse('search'), {
            'q': "'; DROP TABLE books; --"
        })
        self.assertEqual(response.status_code, 200)
    
    def test_xss_protection(self):
        # Test XSS attempts
        response = self.client.post(reverse('comment'), {
            'content': '<script>alert("XSS")</script>'
        })
        self.assertNotIn('<script>', response.content.decode())
```

#### **Security Headers**
```python
# Security middleware
class SecurityMiddleware:
    def __init__(self, get_response):
        self.get_response = get_response
    
    def __call__(self, request):
        response = self.get_response(request)
        response['X-Frame-Options'] = 'DENY'
        response['X-Content-Type-Options'] = 'nosniff'
        response['Referrer-Policy'] = 'same-origin'
        return response
```

---

## 📊 **Analytics & Monitoring**

### **📈 Analytics Implementation**

#### **User Tracking**
```python
# Site visit tracking
class SiteVisit(models.Model):
    timestamp = models.DateTimeField(default=timezone.now)
    user = models.ForeignKey(User, null=True, blank=True, on_delete=models.SET_NULL)
    ip_address = models.GenericIPAddressField(null=True, blank=True)
    path = models.CharField(max_length=512)
    user_agent = models.TextField(null=True, blank=True)
    browser = models.CharField(max_length=32, null=True, blank=True)
    os = models.CharField(max_length=32, null=True, blank=True)
    device_type = models.CharField(max_length=10, choices=DEVICE_CHOICES, default="desktop")
```

#### **Analytics Views**
```python
# Analytics dashboard
@login_required
def analytics_dashboard(request):
    if not request.user.is_staff:
        return redirect('home')
    
    # Get analytics data
    total_users = User.objects.count()
    total_books = Book.objects.count()
    total_visits = SiteVisit.objects.count()
    
    # Daily visits for last 30 days
    daily_visits = SiteVisit.objects.filter(
        timestamp__gte=timezone.now() - timedelta(days=30)
    ).values('timestamp__date').annotate(
        count=Count('id')
    ).order_by('timestamp__date')
    
    context = {
        'total_users': total_users,
        'total_books': total_books,
        'total_visits': total_visits,
        'daily_visits': daily_visits,
    }
    
    return render(request, 'admin/analytics_dashboard.html', context)
```

### **🔍 Monitoring Setup**

#### **Error Monitoring**
```python
# Error logging
import logging

logger = logging.getLogger(__name__)

def handle_error(request, error):
    logger.error(f"Error occurred: {error}")
    # Send notification to admin
    send_error_notification(error)
```

#### **Performance Monitoring**
```python
# Performance tracking
import time
from django.utils.deprecation import MiddlewareMixin

class PerformanceMiddleware(MiddlewareMixin):
    def process_request(self, request):
        request.start_time = time.time()
    
    def process_response(self, request, response):
        if hasattr(request, 'start_time'):
            duration = time.time() - request.start_time
            if duration > 1.0:  # Log slow requests
                logger.warning(f"Slow request: {request.path} took {duration:.2f}s")
        return response
```

---

## 🚀 **Deployment Guide**

### **🌐 Production Deployment**

#### **Server Requirements**
```bash
# Minimum server specifications
- CPU: 2 cores
- RAM: 4GB
- Storage: 50GB SSD
- OS: Ubuntu 20.04 LTS
- Python: 3.11+
- Database: PostgreSQL 13+
```

#### **Environment Setup**
```bash
# Update system
sudo apt update && sudo apt upgrade -y

# Install Python and dependencies
sudo apt install python3 python3-pip python3-venv nginx postgresql

# Install additional packages
sudo apt install libpq-dev python3-dev
```

#### **Application Deployment**
```bash
# Clone repository
git clone https://github.com/kaleemullahkhan786/Public-Library-Bagarji.git
cd Public-Library-Bagarji

# Create virtual environment
python3 -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Configure environment
cp env.example .env
nano .env  # Edit with production settings

# Database setup
sudo -u postgres createdb library_db
sudo -u postgres createuser library_user
sudo -u postgres psql -c "ALTER USER library_user PASSWORD 'your_password';"
sudo -u postgres psql -c "GRANT ALL PRIVILEGES ON DATABASE library_db TO library_user;"

# Run migrations
python manage.py migrate

# Create superuser
python manage.py createsuperuser

# Collect static files
python manage.py collectstatic

# Test application
python manage.py runserver 0.0.0.0:8000
```

#### **Gunicorn Configuration**
```python
# gunicorn.conf.py
bind = "127.0.0.1:8000"
workers = 3
worker_class = "sync"
worker_connections = 1000
max_requests = 1000
max_requests_jitter = 50
timeout = 30
keepalive = 2
```

#### **Nginx Configuration**
```nginx
# /etc/nginx/sites-available/library
server {
    listen 80;
    server_name yourdomain.com www.yourdomain.com;
    
    location = /favicon.ico { access_log off; log_not_found off; }
    
    location /static/ {
        root /var/www/library;
    }
    
    location /media/ {
        root /var/www/library;
    }
    
    location / {
        include proxy_params;
        proxy_pass http://127.0.0.1:8000;
    }
}
```

#### **Systemd Service**
```ini
# /etc/systemd/system/library.service
[Unit]
Description=Library Gunicorn daemon
After=network.target

[Service]
User=www-data
Group=www-data
WorkingDirectory=/var/www/library
ExecStart=/var/www/library/venv/bin/gunicorn --config gunicorn.conf.py public_library_project.wsgi:application
ExecReload=/bin/kill -s HUP $MAINPID
KillMode=mixed
TimeoutStopSec=5
PrivateTmp=true

[Install]
WantedBy=multi-user.target
```

### **🔒 SSL Configuration**

#### **Let's Encrypt SSL**
```bash
# Install Certbot
sudo apt install certbot python3-certbot-nginx

# Obtain SSL certificate
sudo certbot --nginx -d yourdomain.com -d www.yourdomain.com

# Auto-renewal
sudo crontab -e
# Add: 0 12 * * * /usr/bin/certbot renew --quiet
```

### **📊 Monitoring Setup**

#### **Log Management**
```bash
# Log rotation
sudo nano /etc/logrotate.d/library

/var/log/library/*.log {
    daily
    missingok
    rotate 52
    compress
    delaycompress
    notifempty
    create 644 www-data www-data
}
```

---

## ❓ **FAQ & Troubleshooting**

### **🤔 Frequently Asked Questions**

#### **General Questions**

**Q: How do I reset my password?**
A: Click "Forgot Password" on the login page and follow the email instructions.

**Q: Can I download books for offline reading?**
A: Yes, most books are available for PDF download. Look for the download button on book detail pages.

**Q: How do I report inappropriate content?**
A: Use the "Report" button on any content page or contact the administrator directly.

**Q: Is the library free to use?**
A: Yes, the library is completely free for all users.

#### **Technical Questions**

**Q: What browsers are supported?**
A: Chrome, Firefox, Safari, Edge (latest versions)

**Q: Do I need to install any software?**
A: No, the library works entirely in your web browser.

**Q: Can I access the library on mobile?**
A: Yes, the website is fully responsive and works on all mobile devices.

**Q: How do I enable notifications?**
A: Allow notifications when prompted by your browser.

### **🔧 Troubleshooting Guide**

#### **Common Issues**

**Issue: Can't log in**
```bash
# Solution 1: Clear browser cache
# Solution 2: Check email verification
# Solution 3: Reset password
```

**Issue: Books not loading**
```bash
# Solution 1: Check internet connection
# Solution 2: Clear browser cache
# Solution 3: Try different browser
```

**Issue: Upload not working**
```bash
# Solution 1: Check file size (max 50MB)
# Solution 2: Check file format (PDF, JPG, PNG)
# Solution 3: Try smaller file
```

#### **Admin Issues**

**Issue: Admin panel not accessible**
```bash
# Check user permissions
python manage.py shell
>>> from django.contrib.auth.models import User
>>> user = User.objects.get(username='your_username')
>>> user.is_staff = True
>>> user.is_superuser = True
>>> user.save()
```

**Issue: Static files not loading**
```bash
# Collect static files
python manage.py collectstatic

# Check file permissions
sudo chown -R www-data:www-data /var/www/library/staticfiles/
```

**Issue: Database errors**
```bash
# Check database connection
python manage.py dbshell

# Run migrations
python manage.py migrate

# Check for pending migrations
python manage.py showmigrations
```

---

## 📞 **Support & Contact**

### **🎯 Getting Help**

#### **Documentation Resources**
- **User Guide**: This wiki
- **API Documentation**: `/api/docs/`
- **Video Tutorials**: YouTube channel
- **Community Forum**: Discord server

#### **Contact Information**
- **Email**: publiclibrarybagarji@gmail.com
- **Phone**: +92 3147121270
- **WhatsApp**: +92 3147121270
- **Address**: Bagarji, Sukkur, Sindh, Pakistan

#### **Support Channels**
- **Technical Support**: Email with subject "Technical Issue"
- **Feature Requests**: Email with subject "Feature Request"
- **Bug Reports**: Email with subject "Bug Report"
- **General Inquiries**: Email with subject "General Inquiry"

### **🛠️ Custom Development**

#### **Customization Services**
- **Theme Customization**: Brand-specific design
- **Feature Development**: Custom functionality
- **Integration Services**: Third-party integrations
- **Training Programs**: Staff training

#### **Pricing**
- **Basic Customization**: $500 - $1000
- **Advanced Features**: $1000 - $3000
- **Complete Custom Solution**: $3000+
- **Maintenance & Support**: $100/month

---

<div align="center">

## 🎉 **Thank You for Using Public Library Bagarji!**

**We hope this wiki helps you make the most of our library management system.**

[![Documentation](https://img.shields.io/badge/Back%20to%20Top-↑-blue?style=for-the-badge)](#-public-library-bagarji---complete-wiki-documentation)
[![Contact](https://img.shields.io/badge/Contact%20Support-📞-green?style=for-the-badge)](mailto:publiclibrarybagarji@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub%20Repository-📁-orange?style=for-the-badge)](https://github.com/kaleemullahkhan786/Public-Library-Bagarji)

**🌟 Knowledge is Power - Share it with the World! 🌟**

---

*Last Updated: July 2025 | Version: 1.0.0 | Maintained by: Public Library Bagarji Team*

</div> 