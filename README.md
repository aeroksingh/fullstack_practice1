# Fullstack Practice 1

A full-stack web application project with a Django backend and React + Vite frontend.

## 📋 Project Overview

This is a practice project demonstrating a complete full-stack application architecture with:
- **Backend**: Django REST API with PostgreSQL database
- **Frontend**: React application built with Vite
- **Deployment**: Configured for Choreo platform deployment

## 🛠️ Technologies Used

### Backend
- Python 3.x
- Django 4.2.7
- Django REST Framework 3.14.0
- Django CORS Headers 4.3.1
- PostgreSQL (psycopg2-binary 2.9.9)
- Gunicorn 21.2.0
- Python-dotenv 1.0.0
- Whitenoise 6.6.0

### Frontend
- React 18.3.1
- Vite 5.4.10
- React Router DOM 7.0.2
- Axios 1.7.9
- ESLint for code linting

## 📁 Project Structure

```
fullstack_practice1/
├── backend/           # Django backend application
│   ├── api/          # API app
│   ├── backend/      # Django project settings
│   ├── manage.py     # Django management script
│   ├── requirements.txt
│   └── Procfile      # Deployment configuration
├── frontend/         # React frontend application
│   ├── src/         # Source files
│   ├── public/      # Static assets
│   ├── package.json
│   └── vite.config.js
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- Python 3.x
- Node.js and npm
- PostgreSQL (for production)

### Backend Setup

1. Navigate to the backend directory:
```bash
cd backend
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Set up environment variables:
Create a `.env` file with necessary configuration (database credentials, secret key, etc.)

5. Run migrations:
```bash
python manage.py migrate
```

6. Start the development server:
```bash
python manage.py runserver
```

The backend API will be available at `http://localhost:8000`

### Frontend Setup

1. Navigate to the frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

The frontend will be available at `http://localhost:5173`

## 📝 Available Scripts

### Backend
- `python manage.py runserver` - Start development server
- `python manage.py migrate` - Run database migrations
- `python manage.py makemigrations` - Create new migrations
- `python manage.py createsuperuser` - Create admin user

### Frontend
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run lint` - Run ESLint
- `npm run preview` - Preview production build

## 🌐 Deployment

This project is configured for deployment on the Choreo platform with:
- Procfile for backend process management
- Gunicorn as WSGI server
- Whitenoise for static file serving
- PostgreSQL database support

## 🔧 Configuration

### CORS Setup
The backend is configured with Django CORS Headers to allow frontend-backend communication. Update `CORS_ALLOWED_ORIGINS` in settings as needed.

### Database
The project supports both SQLite (development) and PostgreSQL (production). Configure via environment variables.

## 📄 License

This is a practice project for learning purposes.

## 👤 Author

aeroksingh

---

**Note**: This is a practice project created for learning full-stack development with Django and React.
