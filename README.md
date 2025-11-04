# Secure-Call

Secure-Call is a Python-based project designed to provide a secure interface for system calls. It includes features for authentication, logging, and form handling, and is built with modularity and extensibility in mind.

## 📂 Project Folder Structure

```text
System-Call-Monitoring-Dashboard/
│
├── app/
│   ├── __init__.py                # Initializes Flask app, database, and blueprints
│   ├── models.py                  # Database models (SystemCallLog, User, etc.)
│   ├── forms.py                   # Flask-WTF forms for login/register (if any)
│   │
│   ├── routes/
│   │   ├── __init__.py
│   │   ├── auth.py                # Handles user authentication and profile routes
│   │   ├── system_calls.py        # Handles system call logs, APIs, and chart data
│   │   ├── dashboard.py           # Dashboard display logic
│   │
│   ├── static/
│   │   ├── css/
│   │   │   └── style.css          # Custom CSS overrides for Bootstrap
│   │   ├── js/
│   │   │   ├── chart.js           # Chart utilities and reusable functions
│   │   │   └── main.js            # Custom frontend scripts
│   │   ├── img/
│   │   │   └── logo.png           # Project or institute logo (optional)
│   │
│   ├── templates/
│   │   ├── layout.html            # Base layout template (Bootstrap + Navbar)
│   │   ├── dashboard.html         # Dashboard page with activity charts
│   │   ├── login.html             # Login form page
│   │   ├── register.html          # Signup page (optional)
│   │   ├── logs.html              # System logs and history view
│   │   └── error.html             # Error handling templates (404, 500, etc.)
│
├── instance/
│   └── database.db                # SQLite database file (auto-created)
│
├── migrations/                    # Alembic migrations (if using Flask-Migrate)
│
├── tests/
│   ├── test_routes.py             # Unit tests for routes
│   ├── test_models.py             # Unit tests for models
│
├── .gitignore                     # Files and folders ignored by Git
├── requirements.txt               # List of Python dependencies
├── config.py                      # Configuration file (DB URI, secret keys)
├── run.py                         # Entry point to start the Flask app
├── README.md                      # Project documentation
└── LICENSE                        # (Optional) License file if public


## Features

- **Authentication**: Secure user authentication is implemented in [`auth.py`](auth.py).
- **Logging**: Comprehensive logging utilities are available in [`logger.py`](logger.py).
- **Form Handling**: Forms are managed and validated in [`forms.py`](forms.py).
- **Secure System Calls**: System calls are securely handled in [`system_calls.py`](system_calls.py).
- **HTML Templates**: Predefined templates for the user interface are located in the `templates/` directory.
- **Static Assets**: CSS and JavaScript files are stored in the `static/` directory.

## Installation

1. Clone the repository:
   ```bash
   git clone <https://github.com/Adityayadav7567/secure-system-call.git>
   cd secure-syscall-interface
   ```

2. Set up the virtual environment:
   ```bash
   python -m venv .pythonlibs
   source .pythonlibs/bin/activate  # On Windows, use .pythonlibs\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the application:
   ```bash
   python main.py
   ```

## Usage

- Access the application via the provided URL after running `main.py`.
- Use the dashboard to execute secure system calls and manage forms.

 

 
