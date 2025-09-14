# Drupal 10 News Portal

This is a **Drupal 10 project** built locally on **XAMPP**.  

## Requirements
- XAMPP (PHP 8.1+, Apache, MySQL/MariaDB)
- phpMyAdmin (bundled with XAMPP)

---

## Setup Instructions

### 1. Clone Project
Download files and DB from this release https://github.com/tussh/News-Portal/releases/tag/V1.0

download and copy this folder inside your XAMPP `htdocs` folder:
C:\xampp\htdocs\news_portal


### 2. Import Database
1. Start XAMPP (Apache + MySQL).  
2. Open [http://localhost/phpmyadmin](http://localhost/phpmyadmin).  
3. Create a new database `news_portal`.  
4. Import `database/news_portal.sql` into this DB.  

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

## Default Credentials for Admin and Editor User Login Check.
- **Admin username**: `Admin`  
- **Admin password**: `News@123456`  
- **Editor username**: 'Editor'
- **Editor password**: 'News@123456

---
## Project Status & Notes

All the required **functionalities from the assessment have been implemented and are working as expected**:
- User roles and permissions (Admin, Content Editor)
- News content type with taxonomy category restriction (max 3)
- News detail page layout and recently added slider
- Homepage with Top 10, Breaking, and Latest news sliders
- News listing page with pagination
- Sidebar categories
- Static pages
- Multilingual (English & Arabic)
- SEO-friendly URLs
- 404 error page

⚠️ **Note on UI/Styling**  
The primary focus was on completing the functionality within the given deadline.  
- You may notice **minor CSS/UI issues** (especially on responsiveness and desktop view).  
- These are not breaking issues – they were planned for refinement, but due to parallel project tasks and strict timelines, complete polish on UI wasn’t possible.  
- Functionality is stable, and UI adjustments can be addressed in the next iteration.

✅ Rest assured, **all assessment requirements are met and working**.

Thank you.
