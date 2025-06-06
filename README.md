# Bill-Tracker
Bill Tracker (DETS) is a PHP-MySQL web application designed to help users log, manage, and analyze their personal daily expenses. It provides powerful filters for viewing reports by date, month, or year, with a secure login system and intuitive dashboard.

## 🌟 Key Features
- ✅ Secure user registration and logi
- 🧾 Add and manage daily expenses
- 📊 View reports:
- Date-wise
  - Month-wise
  - Year-wise
- Detailed reports for analysis
 - 🔐 Change and reset password functionality
 - 🖥️ Fully responsive dashboard interface
 - 📦 MySQL-based backend with salary integration

## 🗂️ Project Structure Overview
```
dets/
├── assets/                    # Images, icons, logos
├── css/                       # Stylesheets
├── fonts/                     # Web fonts
├── includes/                 # Shared files (dbconn.php, session.php)
├── js/                        # Scripts
├── sass/                      # SCSS styles
├── tables/                    # Data tables for reporting
├── add-expense.php
├── dashboard.php
├── index.php                  # Landing page (login)
├── register.php               # User signup
├── logout.php
├── forgot-password.php
├── reset-password.php
├── change-password.php
├── manage-expense.php
├── user-profile.php
├── expense-[date|month|year]wise-reports[.php|-detailed.php]
SQL File/
└── detsdb.sql                 # MySQL database schema
```

## 🧠 Database Details (detsdb.sql)
- tbluser: stores user details and hashed passwords
- tblexpense: logs expenses with item, amount, date, and user reference
Includes support for:
- Auto-incremented IDs
- Timestamped records
- Sample user data for quick testing

## 🚀 How to Set Up Locally
### 1. Clone the Project
bash
```
git clone https://github.com/yourusername/dets.git
```
### 2. Import the Database
- Open phpMyAdmin
- Create a database named detsdb
- Import detsdb.sql

### 3. Configure Database Connection
In includes/dbconn.php (or similar):
php
```
$host = "localhost";
$user = "root";
$password = "";
$dbname = "detsdb";
```
### 4. Run on Local Server
Place the project in htdocs/ (for XAMPP) and open:
```
http://localhost/dets/
```

## 🔑 Default Credentials
Email	            Password

meena@gmail.com	    1234

raj@gmail.com	      123

## 📌 Notes
- Built using PHP 7+, MySQL, HTML/CSS, JavaScript
- Passwords are MD5-hashed (consider switching to bcrypt in production)
- Designed for academic and personal finance tracking

