# 🐾 Pet Clinic Management System — Spring Boot MVC

A Spring Boot MVC web application for managing pet owners, pets, vets, and visits.  
This project demonstrates layered architecture using Spring MVC, Thymeleaf, and JPA.

---

## 🚀 Features

- Owner management
- Pet registration
- Visit scheduling
- Vet management
- Specialty mapping
- Thymeleaf UI
- Form validation
- MVC architecture
- JPA entity relationships

---

## 🧱 Architecture

Spring MVC layered pattern:

Controller → Service → Repository → Database → Thymeleaf View

---

## 🛠 Tech Stack

- Java 17+
- Spring Boot
- Spring MVC
- Spring Data JPA
- Thymeleaf
- H2 / MySQL (depending on config)
- Maven

---

## 📦 Core Modules

- Owners
- Pets
- Visits
- Vets
- Specialties

---

## 🔄 Application Flow

1. User opens web UI
2. Controller handles request
3. Service executes business logic
4. Repository fetches data
5. Entities mapped via JPA
6. Thymeleaf renders HTML view

---

## 🧪 Demo Flow

Find Owner → Add Owner → Add Pet → Schedule Visit → View Vet List

---

## ▶️ Run Project

Using Maven:

```
mvn spring-boot:run
```

Or run main class:

```
PetClinicApplication.java
```

---

## 🌐 Access Application

Open browser:

```
http://localhost:8080
```

---

## 📚 Learning Outcomes

- Spring MVC architecture
- Controller mappings
- Form binding
- Thymeleaf templates
- JPA relationships
- Layered design pattern

---

## 👨‍💻 Project Type

Spring Boot MVC reference application used to study and practice layered architecture and entity relationships.

---

## 👨‍💻 Author

Koushik Maddi
