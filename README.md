# 🐍 Demo Project for WTForms - Day 61

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://www.python.org/downloads/)
[![Flask Version](https://img.shields.io/badge/flask-2.0%2B-green.svg)](https://flask.palletsprojects.com/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/krishpatel-dev/FlaskWTFormsDemo/graphs/commit-activity)

This repository contains a Flask web application that demonstrates form validation, authentication, and secure login systems using WTForms and Bootstrap.

## 📋 Table of Contents
- [Project List](#-project-list)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Usage](#usage)
- [Project Details](#-project-details)
- [Testing](#-testing)
- [Contributing](#-contributing)

## 🚀 Project List

| # | File | Description |
|---|------|-------------|
| 1 | [main.py](./main.py) | Flask application with WTForms login system and authentication |
| 2 | [templates/base.html](./templates/base.html) | Base HTML template with Bootstrap integration |
| 3 | [templates/index.html](./templates/index.html) | Welcome page with login navigation |
| 4 | [templates/login.html](./templates/login.html) | Login form with validation |
| 5 | [templates/success.html](./templates/success.html) | Success page after successful login |
| 6 | [templates/denied.html](./templates/denied.html) | Access denied page for failed login attempts |

## 🛠 Getting Started

### Prerequisites
- Python 3.8 or higher
- Basic understanding of Flask and web development
- pip package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/krishpatel-dev/FlaskWTFormsDemo.git
   cd FlaskWTFormsDemo
   ```

2. **Set up a virtual environment (recommended)**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install flask flask-wtf flask-bootstrap5 wtforms email-validator
   ```

### Usage

Run the Flask application:
```bash
python main.py
```

Then open your browser and navigate to:
- Home page: http://localhost:5001
- Login page: http://localhost:5001/login

**Test Credentials:**
- Email: `admin@email.com`
- Password: `12345678`

## 📚 Project Details

### 1. Main Application (main.py)
- **Purpose**: Flask web application with secure login system
- **Features**:
  - WTForms integration for form validation
  - Bootstrap5 for responsive UI design
  - CSRF protection for security
  - Email and password validation
  - Custom error messages
  - Session management

### 2. Base Template (templates/base.html)
- **Functionality**:
  - Bootstrap CSS integration
  - Responsive design with viewport meta tag
  - Template inheritance structure
  - Dynamic title and content blocks

### 3. Welcome Page (templates/index.html)
- **Features**:
  - Bootstrap jumbotron for hero section
  - Navigation to login page
  - Responsive layout
  - Clean, modern UI design

### 4. Login Form (templates/login.html)
- **Authentication Features**:
  - Email validation with format checking
  - Password length validation (minimum 8 characters)
  - CSRF token protection
  - Automatic form rendering with Bootstrap5
  - Error message display

### 5. Success Page (templates/success.html)
- **Features**:
  - Displays after successful authentication
  - Embedded Rick Roll GIF for fun
  - Container-based layout

### 6. Access Denied Page (templates/denied.html)
- **Features**:
  - Displays for failed login attempts
  - Embedded funny dog GIF
  - Clear access denied messaging

## 🧪 Testing

You can test the application with different scenarios:

```bash
# Start the application
python main.py

# Test successful login
# Navigate to http://localhost:5001/login
# Email: admin@email.com
# Password: 12345678

# Test failed login
# Use incorrect email or password
# Should redirect to denied.html

# Test form validation
# Try invalid email format
# Try password shorter than 8 characters
# Should show validation errors
```

**Test Cases:**
1. **Valid Login**: Use correct credentials → Success page
2. **Invalid Email**: Use wrong email format → Validation error
3. **Short Password**: Use password < 8 chars → Validation error
4. **Wrong Credentials**: Use valid format but wrong values → Access denied
5. **Empty Fields**: Submit empty form → Required field errors

## 🤝 Contributing

Contributions are welcome! Here's how you can contribute:

1. Fork the repository
2. Create a new branch (git checkout -b feature/amazing-feature)
3. Commit your changes (git commit -m 'Add some amazing feature')
4. Push to the branch (git push origin feature/amazing-feature)
5. Open a Pull Request

## 📝 Learning Objectives

This project demonstrates:
- Flask web framework fundamentals
- WTForms for form handling and validation
- Bootstrap5 for responsive UI design
- CSRF protection and security best practices
- Template inheritance in Jinja2
- Session management and authentication
- Error handling and user feedback

---

<div align="center">
  Made with ❤️ and ☕ by <b>Krish</b>
</div>
