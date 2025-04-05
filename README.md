# 🏋️ RepTrack

RepTrack is a RESTful API built with Spring Boot that helps users log, manage, and track their workouts and exercises over time. Designed with scalability and gym integration in mind, this backend will eventually power a full-stack fitness tracking platform for both users and gym owners.

---

## ⚙️ Tech Stack

- **Java 17+**
- **Spring Boot 3**
- **PostgreSQL**
- **JPA / Hibernate**
- **Docker + Docker Compose**
- **Maven**

---

## 🚀 Getting Started

### 🐳 Prerequisites

- Docker installed
- Java 17+
- Maven (or use `./mvnw` wrapper)

### 🔧 Run the app locally

1. **Start PostgreSQL via Docker**

   ```bash
   docker-compose up -d
   ```

2. **Run Spring Boot API**

   ```bash
   ./mvnw spring-boot:run
   ```

3. **API will be available at:**

   ```
   http://localhost:8080/api/v1/exercises
   ```

---

## 📬 API Endpoints

| Method | Endpoint                               | Description                      |
|--------|----------------------------------------|----------------------------------|
| GET    | `/api/v1/exercises`                    | Get all exercises                |
| POST   | `/api/v1/exercises`                    | Add a new exercise               |
| PUT    | `/api/v1/exercises/{id}`               | Update exercise by ID            |
| DELETE | `/api/v1/exercises/{id}`               | Delete exercise by ID            |
| GET    | `/api/v1/workout-logs`                 | Get all workout logs             |
| POST   | `/api/v1/workout-logs`                 | Add a new workout log            |
| PUT    | `/api/v1/workout-logs/{workoutlogId}`  | Update workout log by ID         |
| DELETE | `/api/v1/workout-logs/{workoutlogId}`  | Delete workout log by ID         |

---

## ✅ Current Progress

- [x] Spring Boot API scaffolding
- [x] PostgreSQL configured using Docker
- [x] Exercise API
- [x] Workout-logs API
- [x] API tested using Postman
- [ ] JWT-based Authentication
- [ ] User roles: User & Gym Owner
- [ ] Analytics / Progress tracking
- [ ] React frontend integration

---

## 📈 Planned Features

- Secure endpoints with JWT Auth
- Create separate dashboard views for gym owners and users
- Integrate exercise recommendation system based on available equipment
- Frontend client in React + TypeScript
- Deployment via Render / Railway / EC2

---

## 📂 Project Structure

```
reptrack/
├── backend/                             
│   ├── src/
│   │   ├── main/java/com/reptrack/api/... 
│   │   └── test/java/com/reptrack/api/... 
│   ├── pom.xml                             
│   ├── mvnw                                
│   └── mvnw.cmd                            
│
├── frontend/                            
│   └── (to be implemented)
│
├── .gitignore                             
├── .gitattributes                         
├── docker-compose.yml                     
├── LICENSE                               
└── README.md                                 
```

---

## 📄 License

MIT License — see [`LICENSE`](./LICENSE) for details.

---

## 🙋‍♂️ Author

Built by **Kevin Ma**

Connect with me on [GitHub](https://github.com/kevindangkhoama) or [LinkedIn](https://www.linkedin.com/in/kevin-dang-khoa-ma/) ✌️
