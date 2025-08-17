## Arham Khan-160923733075
# Task Manager API (Spring Boot)


## Author: Arham Ahmed Khan (160923733075)

# 📖 Project Overview

The Task Manager API is a RESTful web service built with Spring Boot.
It helps in managing daily tasks with fields like:

📝 Title

📄 Description

⏰ Deadline

🔼 Priority

📊 Status

This project demonstrates CRUD operations, clean project structuring, and REST API best practices.

# 🛠 Tech Stack

Backend: Java 22, Spring Boot 3.x

Build Tool: Maven 3.9+

Database: In-Memory (HashMap, can be extended to MySQL/Postgres)

Testing Tools: Postman / cURL

IDE Recommended: IntelliJ IDEA / Eclipse

# <u>✨ Features</u>

#### ✔ Create a new task
#### ✔ Retrieve all tasks or by ID
#### ✔ Update existing task details
#### ✔ Delete tasks
#### ✔ Simple & extendable architecture

# <u>📂 Project Structure</u>
TaskManager/
│── pom.xml
└── src/
    └── main/
        └── java/
            └── com/example/taskmanager/
                ├── controller/TaskController.java   # REST endpoints
                ├── model/Task.java                  # Data model
                └── service/TaskService.java         # Business logic

# <u>🚀 Setup & Run</u>

Clone the repository

git clone https://github.com/your-repo/TaskManager.git
cd TaskManager


Build the project

mvn clean install


Run the application

mvn spring-boot:run


#### 👉 Or run TaskManagerApplication.java directly from IDE

Open http://localhost:8080

# <u>📍 Example Requests</u>
### ➕ Create Task
## POST /tasks
{
  "title": "Learn Spring",
  "description": "Build REST API",
  "deadline": "2025-08-20",
  "priority": "High",
  "status": "Pending"
}

## 📜 Get All Tasks
curl http://localhost:8080/tasks

### ✏️ Update Task
## PUT /tasks/1
{
  "title": "Learn Spring Boot",
  "description": "REST + Swagger",
  "deadline": "2025-08-25",
  "priority": "Medium",
  "status": "Completed"
}

## ❌ Delete Task
curl -X DELETE http://localhost:8080/tasks/1

# <u>🔮 Future Enhancements</u>

Connect with MySQL/Postgres for persistence

Add Swagger/OpenAPI documentation

Implement authentication & user accounts

Deploy on cloud (Heroku/AWS)

# <u>👨‍🎓 Author</u>

Arham Ahmed Khan
🎓 Internship Project Submission
📌 Roll No: 160923733075

#### 📖 This project is a demonstration of API design, Spring Boot development, and clean code practices.
