# 🐾 Spring PetClinic Management System

A **full-stack web application** for managing a veterinary clinic — built with **Spring Boot MVC, Thymeleaf, JPA, and MySQL**, featuring a completely redesigned modern UI with multi-language support.

---

## 🚀 Features

- 🐶 **Pet & Owner Management** — Register owners, add pets, track history
- 👨‍⚕️ **Veterinarian Management** — Manage vet profiles and specializations
- 📅 **Visit Records** — Schedule and track pet visits
- 🗄️ **Multi-Database Support** — H2 (dev), MySQL, PostgreSQL via Spring profiles
- 🌍 **Multi-Language (i18n)** — 9 languages supported
- 🎨 **Custom UI Redesign** — Forest green & amber design system using Bootstrap 5
- ✅ **Full CRUD** — Create, Read, Update, Delete for all entities

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Language | Java 17 |
| Framework | Spring Boot 3.x / Spring MVC |
| Template Engine | Thymeleaf |
| ORM | Spring Data JPA / Hibernate |
| Database | MySQL / PostgreSQL / H2 |
| Frontend | Bootstrap 5, HTML, CSS |
| Build Tool | Maven |

---

## 📁 Project Structure

```
src/
├── main/
│   ├── java/
│   │   └── com/petclinic/
│   │       ├── controller/      # MVC controllers
│   │       ├── service/         # Business logic
│   │       ├── repository/      # Spring Data JPA repos
│   │       └── model/           # Entity classes (Owner, Pet, Vet, Visit, PetType)
│   └── resources/
│       ├── templates/           # Thymeleaf HTML templates
│       ├── static/              # CSS, JS, images
│       ├── messages/            # i18n language files (9 languages)
│       └── application.properties
```

---

## 🗃️ Database Schema

```
Owner ──< Pet >── PetType
Pet   ──< Visit >── Vet
Vet   ──< Speciality
```

**JPA Relationships:**
- `Owner` → `Pet` : OneToMany
- `Pet` → `Visit` : OneToMany
- `Vet` → `Speciality` : ManyToMany

---

## ⚙️ Setup & Run

### Prerequisites
- Java 17+
- MySQL 8+ (or use H2 for quick dev)
- Maven 3.8+

### Run with H2 (no setup needed)
```bash
git clone https://github.com/koush-ik/spring-petclinic-management.git
cd spring-petclinic-management
mvn spring-boot:run
# Visit http://localhost:8080
```

### Run with MySQL
```bash
# Create database
CREATE DATABASE petclinic_db;

# Set profile in application.properties
spring.profiles.active=mysql
spring.datasource.url=jdbc:mysql://localhost:3306/petclinic_db
spring.datasource.username=your_username
spring.datasource.password=your_password

mvn spring-boot:run
```

### Switch Database Profile
```bash
# H2 (default - in-memory)
mvn spring-boot:run -Dspring-boot.run.profiles=default

# MySQL
mvn spring-boot:run -Dspring-boot.run.profiles=mysql

# PostgreSQL
mvn spring-boot:run -Dspring-boot.run.profiles=postgres
```

---

## 🌍 Supported Languages

English, Spanish, German, French, Portuguese, Dutch, Italian, Japanese, Korean

---

## 🎨 UI Highlights

- Fully redesigned with **Bootstrap 5**
- Forest green & amber color system
- Responsive layout — works on mobile and desktop
- Dynamic data binding and form validation via Thymeleaf

---

## 👨‍💻 Author

**Koushik Maddi**  
📧 koushikmaddi113@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/koushik-maddi-b365972a6/)  
🎓 B.Tech ECE — IIIT Surat (2022–2026)
