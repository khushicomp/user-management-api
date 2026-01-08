# User Management & Authentication API

A beginner-friendly backend project built using **Node.js, Express, and MongoDB**.  
This API provides user registration, authentication using JWT, and full CRUD operations on users.

---

Features

- User Signup with password hashing
- User Login with JWT Authentication
- Protected Routes
- Fetch All Users (with Pagination)
- Update User Profile
- Delete User
- Centralized Error Handling

---

 Tech Stack

- Node.js
- Express.js
- MongoDB (Atlas)
- Mongoose
- JWT Authentication
- bcryptjs
- Postman

---

Project Structure

user-management-portal
│
├── config
│ └── db.js
├── middleware
│ ├── authMiddleware.js
│ └── errorMiddleware.js
├── models
│ └── User.js
├── routes
│ └── authRoutes.js
├── .env
├── server.js
└── README.md

yaml
Copy code

---

Setup Instructions

1. Clone Repository
```bash
git clone https://github.com/YOUR_USERNAME/user-management-api.git
cd user-management-api
2. Install Dependencies
bash
Copy code
npm install
3. Configure Environment Variables
Create .env file:

ini
Copy code
PORT=5000
MONGO_URI=your_mongodb_atlas_connection_string
JWT_SECRET=your_secret_key
4. Run Server
bash
Copy code
npm run dev
Server will run on:

arduino
Copy code
http://localhost:5000
 API Endpoints
 Authentication
Register User
POST /api/auth/register

json
Copy code
{
  "name": "Khushi",
  "email": "khushi@test.com",
  "password": "123456"
}
Login User
POST /api/auth/login

json
Copy code
{
  "email": "khushi@test.com",
  "password": "123456"
}
  Users (Protected)
Requires Header:

makefile
Copy code
Authorization: Bearer <TOKEN>
Get All Users (Pagination)
GET /api/auth/users?page=1&limit=5

Update User
PUT /api/auth/users/:id

Delete User
DELETE /api/auth/users/:id

 Testing
All APIs were tested using Postman.

Screenshots
(Attach screenshots of working routes here)
<img width="1838" height="986" alt="Screenshot 2026-01-08 232624" src="https://github.com/user-attachments/assets/2aae6bd8-8eee-4214-9fc5-b8bbc78e1c11" />
<img width="1843" height="984" alt="Screenshot 2026-01-08 232749" src="https://github.com/user-attachments/assets/5460dbe6-9475-4d17-a0de-504f0a3d5ca3" />
<img width="1839" height="997" alt="Screenshot 2026-01-08 232920" src="https://github.com/user-attachments/assets/f249c2ad-b0f9-4c53-867a-289c1c42af84" />
<img width="1840" height="989" alt="Screenshot 2026-01-08 233019" src="https://github.com/user-attachments/assets/059c7eaa-0365-452c-bbf4-de688f41c0a7" />
<img width="1844" height="996" alt="Screenshot 2026-01-08 233210" src="https://github.com/user-attachments/assets/ba3e98c5-846b-4cea-8075-7bd43d6776f8" />
<img width="1837" height="992" alt="Screenshot 2026-01-08 233247" src="https://github.com/user-attachments/assets/ebbe52e7-9e33-4135-aae2-c0488400bd61" />
<img width="1839" height="990" alt="Screenshot 2026-01-08 233440" src="https://github.com/user-attachments/assets/76d23922-796d-495e-945b-9d6c062ef1f7" />


Author
Khushi Yuwanathe
Backend Developer Intern

License
This project is for educational purposes.









