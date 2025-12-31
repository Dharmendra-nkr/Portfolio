# Portfolio Website - Flask Application

A personal portfolio website built with Flask.

## Features

- Home page with profile, about section, and contact information
- Projects page showcasing work and case studies
- Responsive design
- Clean and modern UI

## Installation

1. Install Python 3.8 or higher

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## Running the Application

### Development Mode

```bash
python app.py
```

The application will be available at `http://localhost:5000`

### Production Deployment

For production deployment, use a WSGI server like Gunicorn:

```bash
pip install gunicorn
gunicorn -w 4 -b 0.0.0.0:5000 app:app
```

## Project Structure

```
portfolio/
├── app.py                  # Main Flask application
├── requirements.txt        # Python dependencies
├── static/                 # Static files (images, CSS, JS)
│   ├── images/            # Image files
│   └── ...
├── templates/             # HTML templates
│   ├── home.html
│   └── projects.html
└── README.md
```

## Deployment Options

### Option 1: PythonAnywhere
1. Upload your project files
2. Create a virtual environment
3. Install requirements
4. Configure WSGI file

### Option 2: Heroku
1. Add `Procfile`: `web: gunicorn app:app`
2. Push to Heroku
3. Set environment variables

### Option 3: AWS/DigitalOcean
1. Set up a server with Python
2. Install Nginx
3. Configure Gunicorn as a service
4. Set up Nginx as reverse proxy

## License

© 2024 Dharmendra N K R. All rights reserved.
