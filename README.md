💻 Backend Setup (Before Mood Tracking)
This project is a Node.js backend built using Express and MongoDB, designed to support user authentication and prepare for mood-based personalization features.

✅ Features Implemented
🔐 User Authentication (Login/Signup)
Secure registration and login system.

Passwords are hashed using bcryptjs.

JWT tokens are issued on login for secure session management.

Environment variables managed with .env and dotenv.

🗄️ MongoDB Integration
MongoDB database connected via mongoose.

User schema includes:

username

email

hashed password

createdAt timestamp

📁 Clean File Structure
routes/ folder for API routes (authRoutes.js)

controllers/ folder for route logic (authController.js)

models/ folder for database models (User.js)

config/db.js handles MongoDB connection

server.js is the entry point that initializes the Express server and connects all routes

🌐 API Routes
POST /api/auth/register: Register a new user

POST /api/auth/login: Login existing user

Test route GET / to check if the server is running

🛠️ Middleware
express.json() for parsing JSON bodies

cors() to allow cross-origin requests

🚀 Environment-Based Configuration
Uses process.env for secrets like PORT, JWT_SECRET, and MONGO_URI
