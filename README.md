# 📘 Student CGPA REST API

![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

## 📌 Project Overview
This project is a RESTful API built using **Express.js** that manages student academic performance records using an in-memory JSON database. 

The API supports read-only operations (`GET` requests) and strictly follows REST principles, including proper route design and accurate HTTP status codes. No external database is used — all data is temporarily stored in a local JSON array within the project.

---

## 📖 API Documentation

Comprehensive API documentation, including request/response examples and endpoint details, is available on Postman:

👉 **[View Postman Documentation](https://documenter.getpostman.com/view/50839186/2sBXcEmgp5)**

---

## 🎯 Objective
- Build a robust REST API using Express.js.
- Implement strictly read-only `GET` routes.
- Utilize both static and dynamic routing.
- Adhere to REST API design best practices.
- Return appropriate HTTP status codes (e.g., `200 OK`, `404 Not Found`).
- Manage data dynamically via an in-memory JSON array.

---

## 🛠 Tech Stack
- **Runtime:** Node.js
- **Framework:** Express.js
- **Middleware:** CORS
- **Language:** JavaScript (ES6)

---

## 📂 Implemented Routes

| Method | Endpoint | Description | Status Codes |
|--------|----------|-------------|--------------|
| `GET` | `/students` | Retrieves all student records. | `200` |
| `GET` | `/students/topper` | Returns the student with the highest CGPA. | `200`, `404` |
| `GET` | `/students/average` | Returns the average CGPA of all students. | `200` |
| `GET` | `/students/count` | Returns the total count of students. | `200` |
| `GET` | `/students/:id` | Fetches details of a specific student by ID. | `200`, `404` |
| `GET` | `/students/branch/:branchName` | Returns all students from a specified branch (case-insensitive). | `200` |

---

## 🌍 Live API URLs

The project is live and deployed on Render. You can test the endpoints using the base URL below:

**Base URL:** `https://backend-assignment1.onrender.com`

**Sample Endpoints:**
- 🔹 Get All Students: [`/students`](https://backend-assignment1.onrender.com/students)
- 🔹 Get Topper: [`/students/topper`](https://backend-assignment1.onrender.com/students/topper)
- 🔹 Get Average: [`/students/average`](https://backend-assignment1.onrender.com/students/average)
- 🔹 Get Count: [`/students/count`](https://backend-assignment1.onrender.com/students/count)
- 🔹 Get by ID: [`/students/1`](https://backend-assignment1.onrender.com/students/1)
- 🔹 Get by Branch: [`/students/branch/CSE`](https://backend-assignment1.onrender.com/students/branch/CSE)

---

## 💻 Steps to Run Locally

Follow these steps to set up and run the project on your local machine:

**1️⃣ Clone the repository**
```bash
git clone https://github.com/priyabratasahoo780/backend_assignment1.git
```

**2️⃣ Navigate into the project folder**
```bash
cd backend_assignment1
```

**3️⃣ Install dependencies**
```bash
npm install
```

**4️⃣ Start the server**
```bash
npm start
```
> The server will start running at: `http://localhost:3000`

---

## 📁 Project Structure

```text
backend_assignment1/
│
├── index.js           # Main Express server file
├── package.json       # Project metadata & dependencies
├── package-lock.json  # Dependency tree
└── README.md          # Project documentation (You are here!)
```

---

## 📡 HTTP Status Codes Used

| Status Code | Meaning | Usage |
| :---: | :--- | :--- |
| **`200 OK`** | Request successful | Returned when data is successfully retrieved. |
| **`404 Not Found`** | Resource does not exist | Returned when a student or branch is not found. |

---

## 🧠 Key Concepts Implemented
- **RESTful API Design:** Clean and predictable endpoint structure.
- **Routing:** Effective use of static and dynamic routes.
- **Route Parameters:** Utilizing `req.params` for fetching specific data.
- **Array Methods:** Leveraging `reduce`, `filter`, and `find` for data manipulation.
- **Error Handling:** Standardized responses with proper HTTP status codes.
- **Middleware Usage:** Integrating `express.json` and `cors`.