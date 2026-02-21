# Python Web Application

A Flask-based web application built with Python 3.14.

## Features

- ✅ Flask web framework
- ✅ RESTful API endpoints
- ✅ Health check endpoint
- ✅ Modern responsive UI
- ✅ Production-ready with Gunicorn

## Requirements

- Python 3.14
- pip (Python package manager)

## Installation

1. Create a virtual environment:
```bash
python3.14 -m venv venv
```

2. Activate the virtual environment:
```bash
# On macOS/Linux
source venv/bin/activate

# On Windows
venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Running the Application

### Development Mode

```bash
python app.py
```

The application will be available at `http://localhost:8000`

### Production Mode

```bash
gunicorn --bind 0.0.0.0:8000 app:app
```

## API Endpoints

- `GET /` - Main home page
- `GET /api/health` - Health check endpoint
- `GET /api/info` - Application information

## Project Structure

```
azurewebapppython/
├── app.py              # Main application file
├── requirements.txt    # Python dependencies
├── templates/          # HTML templates
│   └── index.html     # Home page template
├── .gitignore         # Git ignore file
└── README.md          # This file
```

## Deployment

This application is ready to be deployed to various platforms including:
- Azure App Service
- Docker containers
- Heroku
- Any Python-compatible hosting service

## License

MIT
