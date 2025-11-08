🛵 Swiggy Microservice  

![Java](https://img.shields.io/badge/Java-17-blue?style=for-the-badge&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.0.4-brightgreen?style=for-the-badge&logo=spring&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-3.8.7-red?style=for-the-badge&logo=apache-maven&logoColor=white)
![GitHub repo](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge&logo=opensourceinitiative&logoColor=black)

📖 Overview  
The Swiggy Microservice is a Java Spring Boot-based backend application designed to manage restaurants, menus, orders, and user authentication securely.  
It provides REST APIs for restaurant operations, menu management, order tracking, and user management, ensuring a scalable microservice architecture with service discovery (Eureka) and secure endpoints.

🧰 Tech Stack  
- Java 17+  
- Spring Boot (Web, Security, Data JPA)  
- MySQL / H2 (Database)  
- Hibernate (JPA)  
- JWT (JSON Web Token) for Authentication  
- Eureka Discovery for Microservice Registration  
- Swagger for API Documentation  
- Lombok for Boilerplate Reduction  
- Maven for Build & Dependency Management  

⚙️ Features  
✅ User Registration & Login (JWT-based Authentication)  
✅ Role-based Access Control (Admin/User)  
✅ Restaurant CRUD Operations  
✅ Menu Management APIs  
✅ Order Placement & Tracking  
✅ Service Discovery with Eureka  
✅ Global Exception Handling  
✅ Data Validation  
✅ Swagger UI for API Testing  

🚀 Getting Started  

1️⃣ **Clone the Repository**  
```bash
git clone https://github.com/yuvi-chavan/microservice-main.git
cd microservice-main

2️⃣ Configure the Database
Edit your src/main/resources/application.properties file:

spring.datasource.url=jdbc:mysql://localhost:3306/swiggy_db
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect
jwt.secret=yourSecretKey
eureka.client.service-url.defaultZone=http://localhost:8761/eureka/

3️⃣ Build & Run the Project

mvn clean install
mvn spring-boot:run


4️⃣ Access the Application

API Base URL: http://localhost:8080

Swagger UI: http://localhost:8080/swagger-ui/index.html

Eureka Dashboard: http://localhost:8761

🧩 API Highlights

Endpoint	Method	Description
/api/auth/register	POST	Register a new user
/api/auth/login	POST	Login and get JWT token
/api/restaurants	GET/POST/PUT/DELETE	Manage restaurant data
/api/menus	GET/POST/PUT/DELETE	Manage menu items
/api/orders	GET/POST	Place and track orders

🧑‍💻 Author
Yuvraj Chavan
💼 Java Backend Developer | 2025 CSE Passout
📫 GitHub: https://github.com/yuvi-chavan
