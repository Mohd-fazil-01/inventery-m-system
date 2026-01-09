Inventory Management System – README
📌 Project Overview
This project is a role-based Inventory Management System built using MERN Stack (MongoDB, Express, React, Node.js). It focuses on secure authentication, role-based access control, product management, and analytics. The system is designed for real-world use with strong security features like 2FA, account freeze, and admin-controlled access.
________________________________________
🔐 Authentication & Security Features
•	Login using Username & Password
•	Login using Gmail (OAuth)
•	Two-Factor Authentication (2FA) using Email OTP
•	Forgot Password with Gmail OTP verification
•	Password encryption using hashing
•	Account freeze after 5 wrong login attempts
•	Frozen accounts can be unlocked only by Admin
•	Secure session management and logout
________________________________________
👥 Role-Based Access Control (RBAC)
The system supports three user roles:
•	Normal User
•	Super User
•	Admin
Each role has different permissions to ensure security and proper access control.
________________________________________
👤 Normal User Capabilities
•	Access dashboard after login
•	Search products by name, color, category, etc.
•	Apply filters for better product search
•	View all products (read-only)
•	Download product data in Excel format
•	Download product images and barcode images
•	Access analytics dashboard with:
o	Pie Chart
o	Bar / Gradient Chart
o	Line Chart
o	One advanced custom chart
________________________________________
🧑‍💼 Super User Capabilities
•	All permissions of Normal User
•	Add new products
•	Edit existing products
•	Delete products
•	Increase or decrease product quantity
•	View individual product history only
•	Filter product history date-wise
________________________________________
👑 Admin Capabilities
•	All permissions of Normal User and Super User
•	User management:
o	Create users
o	View user details
o	Edit user information
o	Delete users
o	Change user passwords
o	Freeze user accounts
o	Unfreeze user accounts
•	View complete system history:
o	Global product history
o	Individual product history
o	Individual user activity history
o	Date-wise filtering
________________________________________
⚙️ Tech Stack & Libraries Used
🔧 Backend (Node.js)
Core Framework & Server
•	express – Server creation and API handling
•	mongoose – MongoDB connection and data modeling
•	dotenv – Environment variable management
•	cors – Frontend-backend communication
Authentication & Security
•	jsonwebtoken – Secure authentication tokens
•	bcrypt / bcryptjs – Password hashing
•	cookie-parser – Cookie handling
Files & Images
•	multer – File and image uploads
•	cloudinary – Cloud-based image storage
Special Utilities
•	bwip-js – Barcode generation
•	nodemailer – Email & OTP sending
•	nodemon – Auto server restart during development
________________________________________
🎨 Frontend (React)
Core & Routing
•	react – User Interface development
•	vite – Fast development and build tool
•	react-router-dom – Client-side routing
State & Data Management
•	axios – API requests
•	@reduxjs/toolkit / react-redux – Global state management
UI, Reports & Utilities
•	chart.js / react-chartjs-2 – Graphs and analytics
•	xlsx – Excel file download and processing
•	react-hot-toast – Notifications and alerts
________________________________________
🚀 Highlights
•	Enterprise-level authentication flow
•	Strong security with admin-controlled access
•	Clean role separation
•	Analytics-driven dashboard
•	Scalable and production-ready architecture
________________________________________
📂 Usage
This project can be used for:
•	Inventory management systems
•	Admin dashboards
•	Secure enterprise applications
•	College final-year or internship projects
________________________________________
🛠️ Installation & Setup Guide
Follow the steps below to run this project locally on your system.
________________________________________
📥 Clone the Repository
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd <PROJECT_FOLDER_NAME>
________________________________________
⚙️ Backend Setup (Node.js)
1.	Go to backend folder:
cd backend
2.	Install backend dependencies:
npm install
3.	Create a .env file in backend folder and add:
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_email_password
4.	Start backend server:
npm run dev
(Using nodemon for development)
________________________________________
🎨 Frontend Setup (React)
1.	Open new terminal and go to frontend folder:
cd frontend
2.	Install frontend dependencies:
npm install
3.	Start frontend development server:
npm run dev
________________________________________
🌐 Access the Application
•	Frontend will run on: http://localhost:5173
•	Backend API will run on: http://localhost:5000
________________________________________
📌 Notes
•	Make sure Node.js and npm are installed
•	MongoDB should be running or MongoDB Atlas should be connected
•	Use correct Gmail credentials for OTP and emails
________________________________________
✅ This README is structured for GitHub and can be directly used as README.md.

