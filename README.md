# Wells Fargo Software Engineering Virtual Experience — Task 2

![Java](https://img.shields.io/badge/Java-17-orange?logo=java) ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen?logo=springboot) ![JPA](https://img.shields.io/badge/JPA-Hibernate-blue) ![Forage](https://img.shields.io/badge/Forage-Wells%20Fargo-red)

## Overview

This repository contains my completed submission for **Task 2** of the [Wells Fargo Software Engineering Virtual Work Simulation](https://www.theforage.com/simulations/wells-fargo/software-engineering-vcu6) on Forage.

The task involved translating a previously designed Entity Relationship Diagram (ERD) into a working Java data model using Spring Boot and JPA/Hibernate.

---

## Task Description

> As a software engineer at Wells Fargo, financial advisors need a system to manage their clients and the securities in each client's portfolio. Task 2 requires implementing the data model designed in Task 1 as Java entity classes within a Spring Boot application.

### What I implemented

- Annotated Java entity classes using `@Entity` (JPA)
- Configured auto-generated primary keys with `@Id` and `@GeneratedValue`
- Defined relationships between entities (`@OneToMany`, `@ManyToOne`, etc.)
- Added constructors, getters, and setters for all attributes
- Ensured the model aligns with the ERD designed in Task 1

---

## Project Structure

```
src/
└── main/
    └── java/
        └── com/wellsfargo/counselor/
            ├── entity/
            │   ├── Advisor.java
            │   ├── Client.java
            │   ├── Portfolio.java
            │   ├── Security.java
            │   └── PortfolioSecurity.java
            └── CounselorApplication.java
```

---

## Entities

| Entity | Description |
|---|---|
| `Advisor` | Financial advisor managing one or more clients |
| `Client` | Client associated with a specific advisor |
| `Portfolio` | Portfolio belonging to a client |
| `Security` | A financial security (stock, bond, etc.) |
| `PortfolioSecurity` | Join entity linking portfolios to securities with purchase details |

---

## Tech Stack

- **Language:** Java 17
- **Framework:** Spring Boot 3.x
- **ORM:** Spring Data JPA / Hibernate
- **Build Tool:** Maven
- **Database:** H2 (in-memory, for development)

---

## Getting Started

### Prerequisites

- Java 17+
- Maven 3.8+

### Run the application

```bash
git clone https://github.com/sattwik-07/wells-fargo-task-2.git
cd wells-fargo-task-2
mvn spring-boot:run
```

The application starts on `http://localhost:8080` by default.

---

## Certificate
<img width="530" height="408" alt="Screenshot 2026-06-06 010013" src="https://github.com/user-attachments/assets/964b3f7d-d236-404f-b699-2e8e06392327" />

Completed the Wells Fargo Software Engineering Virtual Experience Program on Forage.

---

## Acknowledgements

- [Forage](https://www.theforage.com/) for providing the virtual work simulation
- [Wells Fargo](https://www.wellsfargo.com/) for the program content

---

## 👤 Author

Done by **Sattwik** — [GitHub](https://github.com/sattwik-07)
