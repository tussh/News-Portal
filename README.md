# Drupal 10 News Portal

This is a **Drupal 10 project** built locally on **XAMPP**.  

## Requirements
- XAMPP (PHP 8.1+, Apache, MySQL/MariaDB)
- phpMyAdmin (bundled with XAMPP)

---

## Setup Instructions

### 1. Clone Project
download and copy this folder inside your XAMPP `htdocs` folder:

C:\xampp\htdocs\news_portal


### 2. Import Database
1. Start XAMPP (Apache + MySQL).  
2. Open [http://localhost/phpmyadmin](http://localhost/phpmyadmin).  
3. Create a new database `news_portal`.  
4. Import `database/drupal10_database.sql` into this DB.  

---

### 3. Configure settings.php
1. Go to:  
   ```
   sites/default/settings.php
   ```
2. Edit the database credentials:  

```php
$databases['default']['default'] = [
  'database' => 'news_portal',
  'username' => 'root',
  'password' => '',
  'host' => '127.0.0.1',
  'driver' => 'mysql',
  'prefix' => '',
];
```

---

### 4. Access the Site
Open your browser:  
[http://localhost/news_portal](http://localhost/news_portal)  

---

## Default Credentials
- **Admin username**: `Admin`  
- **Admin password**: `News@123456`  
- **Editor username**: 'Editor'
- **Editor password**: 'News@123456

---
Thank you.
