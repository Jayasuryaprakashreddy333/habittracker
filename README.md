# 🌱 Habit Tracker
    A full-stack web application for tracking daily habits, built with a Node.js backend and a React frontend. Users can register, log in, create habits, mark them as completed on specific days, and view progress through charts and analysis.

## 🚀 Features
  - User Authentication: Secure login and registration system.
  - Habit Management: Create, view, and manage personal habits.
  - Daily Tracking: Mark habits as completed for each day.
  - Data Visualization: Weekly and monthly charts analyze
  - Responsive Design: Works on desktop and mobile devices.

## 🛠 Tech Stack
**Backend**
Node.js with Express.js
MongoDB (assumed based on models)
JWT for authentication
bcrypt for password hashing
**Frontend**
React with Vite
Axios for API calls
Chart.js or similar for visualizations (based on chart components)

## ⚙️ Installation
**Prerequisites**
Node.js (v14 or higher)
MongoDB (local or cloud instance)
npm or yarn

**Backend Setup**
1. Navigate to the backend directory:
cd backend
2. Install dependencies:
npm install
3. Set up environment variables (create a .env file):
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
4. Start the server:
npm start

**Frontend Setup**
1. Navigate to the frontend directory:
cd frontend/my-app
2. Install dependencies
npm install
3. Start the development server:
npm run dev

## Usage
Open your browser and go to http://localhost:5173 (or the port shown by Vite).
Register a new account or log in.
Create new habits on the dashboard.
Mark habits as completed using the checkboxes.
View your progress on the Analysis page with weekly and monthly charts.

## API Endpoints
**Authentication**
POST /api/auth/register - Register a new user
POST /api/auth/login - Log in a user
**Habits**
GET /api/habits - Get all habits for the logged-in user
POST /api/habits - Create a new habit
PUT /api/habits/:id - Update a habit
DELETE /api/habits/:id - Delete a habit
**Analysis**
GET /api/analysis - Get habit analysis data

## 📂 Project Structure
habitTracker/
├── backend/
│   ├── middleware/
│   │   └── authMiddleware.js
│   ├── models/
│   │   ├── Habit.js
│   │   └── User.js
│   ├── routes/
│   │   ├── analysis.js
│   │   ├── auth.js
│   │   └── habits.js
│   ├── package.json
│   └── server.js
├── frontend/my-app/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── DayCheckbox.jsx
│   │   │   ├── MonthlyChart.jsx
│   │   │   ├── Navbar.jsx
│   │   │   └── WeeklyChart.jsx
│   │   ├── hooks/
│   │   │   ├── useAnalysis.js
│   │   │   ├── useAuth.js
│   │   │   └── useHabits.js
│   │   ├── pages/
│   │   │   ├── Analysis.jsx
│   │   │   ├── Dashboard.jsx
│   │   │   ├── HabitTable.jsx
│   │   │   ├── Login.jsx
│   │   │   └── Register.jsx
│   │   ├── utils/
│   │   │   └── api.js
│   │   ├── App.jsx
│   │   ├── index.css
│   │   └── main.jsx
│   ├── package.json
│   ├── vite.config.js
│   └── index.html
└── README.md

## Contributing
1. Fork the repository.
2. Create a new branch for your feature.
3. Make your changes and test thoroughly.
4. Submit a pull request.

## License
This project is licensed under the MIT License.