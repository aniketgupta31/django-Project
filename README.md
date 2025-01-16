# Chat Application

This project is a Django-based real-time chat application with user authentication, chat functionality, and a user-friendly interface.

## Features
- User registration and login
- Real-time chat functionality
- Modern and responsive user interface
- Built with Django and WebSockets

## Prerequisites
Make sure you have the following installed:

- Python 3.8+
- pip (Python package manager)
- Virtualenv (optional but recommended)
- SQLite (comes pre-installed with Python)

## Getting Started
Follow these steps to set up and run the project locally.

### 1. Clone the Repository
```bash
git clone <repository_url>
cd chat_app
```

### 2. Create a Virtual Environment (Optional)
It is recommended to use a virtual environment to avoid conflicts.
```bash
python -m venv venv
source venv/bin/activate      # On macOS/Linux
venv\Scripts\activate       # On Windows
```

### 3. Install Dependencies
Install the required Python libraries using the `requirements.txt` file.
```bash
pip install -r requirements.txt
```

### 4. Apply Migrations
Set up the database by applying the migrations.
```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Run the Development Server
Start the Django development server.
```bash
python manage.py runserver
```

The application will be accessible at [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

## Usage
1. **Register a User:** Navigate to the registration page and create a new account.
2. **Login:** Use your credentials to log in.
3. **Start Chatting:** Access the chat interface to begin chatting with other users.

## Project Structure
```
chat_app/
├── chat_app/                 # Project-level settings and configuration
│   ├── settings.py          # Main settings file
│   ├── urls.py              # URL routing
│   ├── asgi.py              # ASGI configuration for WebSocket support
│   └── wsgi.py              # WSGI configuration for deployment
├── users/                    # Django app for user management and chat
│   ├── templates/           # HTML templates
│   ├── static/              # CSS and JavaScript files
│   ├── views.py             # Views for handling logic
│   └── models.py            # Database models
├── manage.py                 # Entry point for Django commands
├── requirements.txt          # Python dependencies
└── db.sqlite3                # SQLite database file
```
