# fullstack-complaint-app

🧾 Full-Stack Complaint Management System
📘 Project Overview

The Complaint Management System (CMS) is a full-stack web application that allows users to register complaints, track their status, and view responses in real time.
It provides an efficient workflow for users, administrators, and service departments to communicate and resolve issues seamlessly.

The system is built using the MERN stack (MongoDB, Express.js, React/HTML/CSS frontend, Node.js backend) with RESTful APIs and secure authentication.

🧩 Tech Stack
Layer	Technology
Frontend	HTML, CSS, JavaScript
Backend	Node.js, Express.js
Database	MongoDB Atlas
Authentication	JWT (JSON Web Tokens)
Tools	Nodemon, dotenv, multer (for uploads), bcryptjs
Hosting (optional)	Render / Vercel / Netlify
⚙️ Project Setup
1. Clone the Repository
git clone https://github.com/gargi411/fullstack-complaint-app.git
cd fullstack-complaint-app

2. Install Backend Dependencies
cd backend
npm install

3. Create Environment File

Inside backend/.env, add your credentials:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key

4. Run the Backend Server
npm run dev


Server will start on: http://localhost:5000

5. Run the Frontend

Open a second terminal and run:

cd frontend
npx http-server -c-1


Frontend will run on: http://127.0.0.1:8080

🔐 Authentication Routes
Method	Endpoint	Description
POST	/api/auth/signup	Register a new user
POST	/api/auth/login	Authenticate user & issue JWT
GET	/api/complaints	Get complaints for logged-in user
POST	/api/complaints	File a new complaint
PUT	/api/complaints/:id	Update complaint status
🧠 Core Features

✅ User registration and login with password encryption
✅ Secure JWT-based authentication
✅ Submit and track complaints in real time
✅ Upload supporting images/documents
✅ Admins can view and update complaint statuses
✅ Clean, responsive UI (light/dark mode supported)

🗃️ Folder Structure
fullstack-complaint-app/
│
├── backend/
│   ├── server.js
│   ├── .env
│   ├── config/
│   │   └── db.js
│   ├── models/
│   │   └── User.js
│   ├── routes/
│   │   ├── auth.js
│   │   └── complaints.js
│   ├── middleware/
│   │   └── authMiddleware.js
│   └── uploads/
│
├── frontend/
│   ├── index.html
│   ├── login.html
│   ├── signup.html
│   ├── style.css
│   ├── script.js
│   └── map.png
│
└── README.md

📸 Screenshots

Add screenshots here (once frontend is styled)

/frontend/screenshots/


Example:

![Login Page](frontend/screenshots/login.png)
![Complaint Dashboard](frontend/screenshots/dashboard.png)

📡 API Testing

Use Postman or Thunder Client to test endpoints.
Include header:

Authorization: Bearer <your_jwt_token>

👩‍💻 Author

Name: Gargi Balamwar
GitHub: @gargi411

Institute: Symbiosis Institute of Technology, Nagpur
Course: Introduction to Full Stack Development

⭐ Future Enhancements

Admin dashboard for analytics

SMS/Email complaint notifications

Complaint prioritization and AI-based categorization

Multi-language support
