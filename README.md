🥗 DietCoach
Your personalized diet companion for India - AI-powered meal planning with responsive UI, authentication, and comprehensive health tracking.

Version License

✨ Features
📱 Responsive Design
Mobile-first design that adapts to all screen sizes
Optimized for phones, tablets, and desktops
🔐 Authentication
Secure user registration and login
JWT token-based authentication
Password encryption with BCrypt
📋 7-Section Navigation
Dashboard - Daily progress tracking with calorie circle and macros
Daily Plan - AI-generated meal plans with swap/re-roll functionality
Meal Log - Multiple logging methods (grams, cups, hand-size, count)
Progress - Weight tracking with weekly summary
Check-In - Weekly progress form with mood and adherence tracking
Coach Assistant - Placeholder for upcoming AI features
Settings - Complete profile management with preferences and logout
🎯 Onboarding
3-step onboarding process
Health profile collection (age, gender, height, weight, activity level)
Goal selection with multiple options
Dietary preferences (veg/non-veg, cooking oil, region)
🛠️ Tech Stack
Frontend
React 18 - Modern UI library
Tailwind CSS - Utility-first CSS framework
Lucide Icons - Beautiful icon library
Axios - HTTP client
Backend
Spring Boot 3.2.0 - Java framework
Spring Security 6 - Authentication & authorization
PostgreSQL - Database (Supabase)
JWT - Token-based authentication
Maven - Build tool
🚀 Getting Started
Prerequisites
Node.js 16+ and npm
Java 17+
Maven 3.6+
PostgreSQL database (or Supabase account)
Installation
1. Clone the repository
git clone https://github.com/Prasathn01/DietCoach.git
cd DietCoach
2. Backend Setup
cd diet-coach-backend

# Create .env file with your database credentials
cat > .env << 'ENV'
DB_URL=jdbc:postgresql://your-db-host:5432/your-db-name
DB_USERNAME=your-username
DB_PASSWORD=your-password
JWT_SECRET=your-secret-key-here
SERVER_PORT=8080
ENV

# Run the backend
mvn spring-boot:run
Backend will start on http://localhost:8080

3. Frontend Setup
cd diet-coach-frontend

# Install dependencies
npm install

# Create .env file
echo "REACT_APP_API_URL=http://localhost:8080" > .env

# Start the development server
npm start
Frontend will start on http://localhost:3000

📦 Deployment
Frontend (Netlify)
Go to Netlify
Import from GitHub
Configure:
Root Directory: diet-coach-frontend
Build Command: npm run build
Publish Directory: build
Environment Variables: REACT_APP_API_URL=<your-backend-url>
Backend (Render)
Go to Render
Create new Web Service
Configure:
Root Directory: diet-coach-backend
Build Command: mvn clean install
Start Command: java -jar target/diet-coach-backend-1.0.0.jar
Add environment variables from .env
📝 Environment Variables
Backend
DB_URL=jdbc:postgresql://host:5432/database
DB_USERNAME=username
DB_PASSWORD=password
JWT_SECRET=your-secret-key
SERVER_PORT=8080
Frontend
REACT_APP_API_URL=http://localhost:8080
🏗️ Project Structure
DietCoach/
├── diet-coach-backend/          # Spring Boot backend
│   ├── src/
│   │   └── main/
│   │       ├── java/
│   │       │   └── com/dietcoach/
│   │       │       ├── controller/
│   │       │       ├── model/
│   │       │       ├── repository/
│   │       │       ├── security/
│   │       │       └── service/
│   │       └── resources/
│   └── pom.xml
│
└── diet-coach-frontend/         # React frontend
    ├── public/
    ├── src/
    │   ├── config/
    │   ├── services/
    │   ├── App.js
    │   └── index.js
    └── package.json
🔒 Security
Passwords are encrypted using BCrypt
JWT tokens for stateless authentication
CORS configured for frontend-backend communication
Environment variables for sensitive data
.env files excluded from Git
📱 Screenshots
Coming soon

🤝 Contributing
This is a private repository. Access is restricted to authorized collaborators only.

📄 License
Private - All rights reserved

👨‍💻 Author
Prasath

GitHub: @Prasathn01
🙏 Acknowledgments
Built with modern web technologies
Designed for the Indian diet and lifestyle
Responsive UI for all devices
Version A1 - Initial Release 🚀
