# Arham Khan-160923733075
Task Manager (Spring Boot)

👩‍💻 Author: ARHAM AHMED KHAN – 160923733075

A simple yet powerful REST API for managing daily tasks with attributes like Title, Description, Deadline, Priority, and Status.
Ideal for learning Spring Boot, REST APIs, and CRUD operations.

✅ Tech Requirements

☕ Java 17+ (Project is configured for Java 22 in pom.xml)

📦 Maven 3.9+

🌐 Internet access (for dependencies)

🧪 (Optional): Postman / cURL for testing

📂 Project Directory
TaskManager/
│── pom.xml
└── src/
    └── main/
        └── java/
            └── com/example/taskmanager/
                ├── controller/TaskController.java
                ├── model/Task.java
                └── service/TaskService.java

🏃 How to Run

1️⃣ Clone repository

git clone https://github.com/your-repo/TaskManager.git
cd TaskManager


2️⃣ Build the project

mvn clean install


3️⃣ Start the application

mvn spring-boot:run


👉 Alternatively, run TaskManagerApplication.java directly in your IDE.

4️⃣ Check if it’s running
Open ➡ http://localhost:8080

🔗 API Endpoints
➕ Create Task

POST /tasks

{
  "title": "Learn Spring",
  "description": "Build REST API",
  "deadline": "2025-08-20",
  "priority": "High",
  "status": "Pending"
}

📜 Get All Tasks

GET /tasks

🔍 Get Task by ID

GET /tasks/{id}

✏️ Update Task

PUT /tasks/{id}

{
  "title": "Learn Spring Boot",
  "description": "REST + Swagger",
  "deadline": "2025-08-25",
  "priority": "Medium",
  "status": "Completed"
}

❌ Delete Task

DELETE /tasks/{id}

🛠 Testing with cURL

📌 Add a Task

curl -X POST http://localhost:8080/tasks \
-H "Content-Type: application/json" \
-d '{"title":"Learn Spring","description":"Build REST API","deadline":"2025-08-20","priority":"High","status":"Pending"}'


📌 Get All Tasks

curl http://localhost:8080/tasks


📌 Get Task by ID

curl http://localhost:8080/tasks/1


📌 Update a Task

curl -X PUT http://localhost:8080/tasks/1 \
-H "Content-Type: application/json" \
-d '{"title":"Learn Spring Boot","description":"REST + Swagger","deadline":"2025-08-25","priority":"Medium","status":"Completed"}'


📌 Delete a Task

curl -X DELETE http://localhost:8080/tasks/1
