# Expense Tracker
## Video Demo
https://youtu.be/4WSFPgOUB7I?si=u7EZcBTsKt2KKby-
## Project Overview
Expense Tracker is a simple expense tracking application based on Flask. It allows users to register, log in, and track their daily expenses. Users can add, edit, and delete expense records and view expense summaries categorized by month and category.

## Features
- **User Registration & Login**: Users can register new accounts and log in.
- **Expense Record Management**:
  - Add expense records (including amount, category, description, and date).
  - Edit existing expense records.
  - Delete expense records.
- **Expense Summary**:
  - Total expenses categorized by month.
  - Total expenses categorized by category.
- **User-Friendly Interface**: Uses Bootstrap and Font Awesome to enhance the interface and provide a good user experience.

## File Structure
Below are the main files of the project and their functions:

### `app.py`
This is the main file of the project, containing all Flask routes and logic. Key functionalities include:
- **User Authentication**: Handles user registration, login, and logout.
- **Expense Record Management**: Handles adding, editing, and deleting expense records.
- **Database Operations**: Uses SQLAlchemy to manage user and expense record data.

### `layout.html`
This is the base template for all pages, including the navigation bar and basic page structure. Key functionalities include:
- **Navigation Bar**: Displays registration, login, and logout links (dynamically shown based on user login status).
- **Page Layout**: Defines the overall page structure and styles.

### `index.html`
This is the homepage after the user logs in, displaying the user's expense records and summary information. Key functionalities include:
- **Expense Record Table**: Displays detailed expense records.
- **Monthly Summary**: Shows total expenses categorized by month.
- **Category Summary**: Shows total expenses categorized by category.

### `login.html`
This is the user login page, containing a login form. Key functionalities include:
- **Login Form**: Users enter their username and password to log in.
- **Error Messages**: Displays corresponding error messages if the username or password is incorrect.

### `register.html`
This is the user registration page, containing a registration form. Key functionalities include:
- **Registration Form**: Users enter a username, password, and confirm password to register.
- **Error Messages**: Displays corresponding error messages if the passwords do not match or the username already exists.

### `add_expense.html`
This is the page for adding expense records, containing a form. Key functionalities include:
- **Expense Form**: Users enter the amount, category, and description to add an expense record.

### `edit_expense.html`
This is the page for editing expense records, containing a pre-filled form. Key functionalities include:
- **Edit Form**: Users modify the amount, category, and description to update an expense record.

### `README.md`
This is the project documentation file, detailing the features, file structure, and design concepts of the project.

## How to Run the Project
1. **Install Dependencies**:
   ```bash
   pip install flask flask-sqlalchemy flask-login
   ```

2. **Initialize the Database**:
   ```bash
   python3
   >>> from app import db
   >>> db.create_all()
   >>> exit()
   ```

3. **Run the Application**:
   ```bash
   python3 app.py
   ```

4. **Access the Application**:
   - Open a browser and visit `http://127.0.0.1:5000`.
   - Register a new user, log in, and start tracking expenses.