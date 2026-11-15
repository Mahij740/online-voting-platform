# 🗳 Online Voting Platform

A full-stack **Online Voting Platform** developed using **Spring Boot**, **Spring Security**, **PostgreSQL**, and **Bootstrap 5**. The application provides a secure and user-friendly interface to manage voters, candidates, voting, election results, and vote history.

---

## 📖 Overview

The Online Voting Platform is designed to digitize the election process by allowing administrators to:

* Register and manage voters
* Add, update, and remove candidates
* Cast votes securely
* View complete vote history
* Display the election winner

The project follows a layered architecture using Spring Boot, REST APIs, Hibernate (JPA), and PostgreSQL.

---

# ✨ Features

* 👤 Voter Registration
* 📋 View Registered Voters
* 🏛 Candidate Management
* 📝 Update Candidate Details
* 🗑 Delete Candidates
* 🗳 Cast Vote
* ✅ One Vote Per Voter Validation
* 📜 Vote History
* 🏆 Election Winner
* ✔ Form Validation
* 🔒 Spring Security
* 🌐 REST APIs
* 💾 PostgreSQL Database Integration
* 📱 Responsive Bootstrap UI

---

# 🛠 Tech Stack

## Backend

* Java 21
* Spring Boot 4
* Spring Web MVC
* Spring Data JPA
* Hibernate
* Spring Security
* Maven

## Frontend

* HTML5
* CSS3
* Bootstrap 5
* Bootstrap Icons
* JavaScript

## Database

* PostgreSQL 18

## Development Tools

* Eclipse IDE
* Git
* GitHub

---

# 📂 Project Structure

```text
online-voting-platform
│
├── src
│   └── main
│       ├── java
│       │   └── com.voting
│       │       ├── config
│       │       ├── controller
│       │       ├── entity
│       │       ├── exception
│       │       ├── repository
│       │       ├── service
│       │       └── OnlineVotingPlatformApplication.java
│       │
│       └── resources
│           ├── static
│           │   ├── css
│           │   ├── js
│           │   ├── index.html
│           │   ├── dashboard.html
│           │   ├── voter.html
│           │   ├── candidate.html
│           │   ├── vote.html
│           │   ├── history.html
│           │   └── winner.html
│           │
│           └── application.properties
│
├── pom.xml
├── README.md
└── screenshots
🚀 Getting Started
1. Clone the Repository
Bash
git clone [https://github.com/Mahij740/online-voting-platform.git](https://github.com/Mahij740/online-voting-platform.git)
2. Open the Project
Import the project into Eclipse IDE as a Maven project.

3. Create PostgreSQL Database
SQL
CREATE DATABASE online_voting;
4. Configure Database
Update your application.properties.

Properties
spring.datasource.url=jdbc:postgresql://localhost:5432/online_voting
spring.datasource.username=YOUR_USERNAME
spring.datasource.password=YOUR_PASSWORD

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

server.port=9999
5. Run the Application
Run:

Plaintext
OnlineVotingPlatformApplication.java
Open:

Plaintext
http://localhost:9999
📋 Modules
🏠 Home Page

📊 Dashboard

👤 Voter Management

🏛 Candidate Management

🗳 Cast Vote

📜 Vote History

🏆 Winner Page

🌐 REST API Endpoints
Voter
Method	Endpoint
POST	/voter/register
GET	/voter
GET	/voter/{id}
DELETE	/voter/{id}
Candidate
Method	Endpoint
POST	/candidate
GET	/candidate
GET	/candidate/{id}
PUT	/candidate/{id}
DELETE	/candidate/{id}
Vote
Method	Endpoint
POST	/vote/{voterId}/{candidateId}
GET	/vote
GET	/vote/{id}
GET	/vote/voter/{voterId}
GET	/vote/candidate/{candidateId}
Winner
Method	Endpoint
GET	/winner
✔ CRUD Operations
Module	Create	Read	Update	Delete
Candidate	✅	✅	✅	✅
Voter	✅	✅	❌	✅
Vote	✅	✅	❌	❌
✔ Validation
The application validates:

Required fields

Email format

Password presence

Duplicate voter registration

One vote per voter

Resource existence

🔒 Security
The application uses Spring Security with:

HTTP Basic Authentication

BCrypt Password Encryption

Protected REST APIs

Public access to frontend pages

🖼 Screenshots
🏠 Home Page
📊 Dashboard
👤 Voter Management
🏛 Candidate Management
🗳 Cast Vote
📜 Vote History
🏆 Election Winner
🚀 Future Enhancements
JWT Authentication

Admin Login

Voter Login

Election Scheduling

Candidate Photos

Live Result Dashboard

Charts & Analytics

Email Notifications

Result Export (PDF/Excel)

👨‍💻 Author
Mahij740

GitHub: https://github.com/Mahij740

⭐ Support
If you found this project useful, consider giving it a ⭐ on GitHub.

📄 License
This project is developed for educational and academic purposes.


### Quick Checklist Before You Push:
1. **Screenshot filenames:** Make sure your 7 new images inside `screenshots/` are named exactly `home.png`, `dashboard.png`, `voter.png`, `candidate.png`, `vote.png`, `history.png`, and `winner.png` (all lowercase `.png`), otherwise GitHub won't render them.
2. **Sanitize `application.properties`:** Change `spring.datasource.password=...` back to `YOUR_PASSWORD` before running `git add .`.
3. **Check `pom.xml`:** Open `pom.xml` briefly to make sure `<groupId>` or `<description>` doesn't still contain `Devaanshhh` (if it's `com.voting`, you're completely good to go).