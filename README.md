# Image-Processing-System
Build a system to efficiently process image data from CSV files.


Python
pycache/
*.py[cod]
*$py.class
*.so
.Python
build/
develop-eggs/
dist/
downloads/
eggs/
.eggs/
lib/
lib64/
parts/
sdist/
var/
wheels/
*.egg-info/
.installed.cfg
*.egg
MANIFEST

Environment
.env
.venv
env/
venv/
ENV/
env.bak/
venv.bak/

IDE
.vscode/
.idea/
*.swp
*.swo

Database
*.db
*.sqlite3

Uploads and processed files
/uploads/
/processed/
/processed_images/

Logs
*.log
logs/

OS
.DS_Store
Thumbs.db


### README.md

# Image Processing System

A complete system to process CSV files containing image URLs, compress images asynchronously, and provide status tracking through APIs.

## Features

- CSV file upload with validation
- Asynchronous image processing
- Progress tracking via API
- Webhook notifications
- Docker containerization
- PostgreSQL database for persistence

## Installation

1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Set up environment variables (copy `.env.example` to `.env`)
4. Run the application: `uvicorn src.app.main:app --reload`

## Docker Setup

1. Ensure Docker and Docker Compose are installed
2. Run: `docker-compose -f docker/docker-compose.yml up --build`

## API Documentation

See [API Documentation](docs/API_Documentation.md) for detailed endpoint information.

## Database Schema

The system uses two main tables:

1. **requests**: Tracks processing requests with status and progress information
2. **products**: Stores individual product processing results

THANK YOU........
