# 📘 Backend Assignment 1
Student CGPA REST API (Read-Only)

📌 Project Overview

This project is a RESTful API built using Express.js that manages student academic performance records using an in-memory JSON database.

The API supports read-only operations (GET requests) and follows REST principles including proper route design and correct HTTP status codes.

No external database is used — all data is stored in a local JSON array inside the project.

🎯 Objective

Build a REST API using Express.js

Implement only GET routes

Use both static and dynamic routes

Follow REST principles

Return proper HTTP status codes

Store data in an in-memory JSON array


🛠 Tech Stack

Node.js

Express.js

CORS

JavaScript (ES6)

📂 Implemented Routes

1️⃣ Get All Students
GET /students

Returns all student records.
Status Code: 200 OK

2️⃣ Get Topper (Highest CGPA)
GET /students/topper

Returns the student with the highest CGPA.
If no students exist → 404 Not Found

3️⃣ Get Average CGPA
GET /students/average

Returns the average CGPA of all students.

4️⃣ Get Total Student Count
GET /students/count

5️⃣ Get Student by ID (Dynamic Route)
GET /students/:id

Returns specific student details.
If student not found → 404 Not Found

6️⃣ Get Students by Branch (Dynamic Route)
GET /students/branch/:branchName

Returns all students from the specified branch (case-insensitive).
Returns empty array if no students match.


🌍 Sample API URLs (After Deployment)

https://your-render-link.onrender.com/students
https://your-render-link.onrender.com/students/topper
https://your-render-link.onrender.com/students/average
https://your-render-link.onrender.com/students/count
https://your-render-link.onrender.com/students/1
https://your-render-link.onrender.com/students/branch/CSE


💻 Steps to Run Locally

1️⃣ Clone the repository
git clone https://github.com/priyabratasahoo780/backend_assignment1.git

2️⃣ Navigate into the project folder
cd backend_assignment1

3️⃣ Install dependencies
npm install

4️⃣ Start the server
npm start

Server will run at:
http://localhost:3000


🚀 Deployment
This project is deployed on Render.

Deployed Link
https://your-render-link.onrender.com


📁 Project Structure

backend_assignment1/
│
├── index.js        # Main server file
├── package.json    # Project configuration
├── package-lock.json
└── README.md       # Project documentation


📡 HTTP Status Codes Used
| Status Code   | Meaning                 |
| ------------- | ----------------------- |
| 200 OK        | Request successful      |
| 404 Not Found | Resource does not exist |


🧠 Key Concepts Implemented

RESTful API design

Static and Dynamic routes

Route parameters (req.params)

Array methods (reduce, filter, find)

Proper HTTP status codes

Middleware usage (express.json, cors)