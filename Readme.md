## Fruit Management App

A Full Stack Application built with FastAPI (Python) for the backend and React.js (Vite) for the frontend.
This project demonstrates seamless communication between a FastAPI REST API and a React client, handling data operations such as fetching and adding fruits in real-time.

## Tech Stack
### Backend

FastAPI (Python 3.9+)

Uvicorn (ASGI Server)

Pydantic (Data validation)

CORS Middleware (Cross-origin communication)

### Frontend

React.js (Vite)

Axios (HTTP client)

Modern JavaScript (ES6+)

## Backend Setup (FastAPI)
🧩 Prerequisites

Python 3.9+

pip (Python package manager)

🛠️ Setup Steps

Navigate to the backend folder:

cd backend


Create and activate a virtual environment:

Windows

python -m venv venv
.\venv\Scripts\activate


Mac/Linux

python3 -m venv venv
source ./venv/bin/activate


Install dependencies:

pip install -r requirements.txt


Run the FastAPI server:

python main.py


API will be available at:
🔗 http://localhost:8000

💻 Frontend Setup (React + Vite)
🧩 Prerequisites

Node.js & npm (Latest LTS recommended)

🛠️ Setup Steps

Navigate to the frontend folder:

cd frontend


Install dependencies:

npm install
npm install axios


Run the development server:

npm run dev


React app will run at:
🔗 http://localhost:3000

🔄 Connecting Frontend & Backend

The React frontend communicates with the FastAPI backend using Axios.

Ensure both servers are running:

FastAPI → http://localhost:8000

React → http://localhost:3000

CORS is enabled on the backend to allow requests from the React origin.

## Features

✅ Fetch fruits from backend
✅ Add new fruits dynamically
✅ Instant UI updates after adding a fruit
✅ Clean and modular React components
✅ API built with modern FastAPI practices

## API Endpoints
Method	Endpoint	Description
GET	/fruits	Fetch all fruits
POST	/fruits	Add a new fruit

## Useful Commands
Command	Description
python main.py	Run FastAPI backend
npm run dev	Run React frontend
pip install -r requirements.txt	Install backend dependencies
npm install	Install frontend dependencies

## Developer Notes

Both services must be running simultaneously.

You can modify the base URL in frontend/src/api.js if the backend runs on a different port.

Use CORS middleware in FastAPI to handle frontend-backend communication.