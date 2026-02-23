# FastAPI + Streamlit Image Upload App
A full‑stack project built with FastAPI (backend) and Streamlit (frontend) that allows users to register/login, upload images or videos, and store metadata in a database. Files are uploaded to ImageKit for cloud storage and delivery.

#FEATURES
User authentication (JWT via FastAPI Users)
File upload (images/videos)
Integration with ImageKit for media hosting
Database persistence with SQLAlchemy
Streamlit frontend for easy interaction

#TECH-STACK
Backend: FastAPI, SQLAlchemy, FastAPI Users
Frontend: Streamlit
Media: ImageKit SDK
Database: (Postgres/MySQL/SQLite — whichever you’re using)
Environment: Python 3.11, uv

#ENVIRONMENT_VARIABLES
IMAGEKIT_PRIVATE_KEY=your_private_key
IMAGEKIT_PUBLIC_KEY=your_public_key
IMAGEKIT_URL_ENDPOINT=https://ik.imagekit.io/your_imagekit_id/
DATABASE_URL=sqlite+aiosqlite:///./test.db   # or your DB connection string

#RUNNING THE PROJECT
# Start backend
uv run uvicorn main:app --reload --port 8000

# Start frontend
uv run streamlit run frontend.py
