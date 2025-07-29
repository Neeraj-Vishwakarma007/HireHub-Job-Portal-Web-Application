💼 HireHub – Job Portal Web Application
A full-featured, role-based job portal system designed to streamline the recruitment lifecycle — from job posting to candidate application — with real-time OTP verification, resume management, and secure authentication using Google reCAPTCHA.

Built during my Java Full Stack Internship, this project showcases practical implementation of Java EE technologies, servlet-based RESTful architecture, database interaction using JDBC, and seamless frontend-backend integration.

🔧 Tech Stack
Frontend:

HTML, CSS, JavaScript, Bootstrap

Backend:

Core Java (Java 11)

Servlet 4.0

JavaMail API

Twilio API (SMS OTP)

Database:

MySQL

Server:

Apache Tomcat 9

Security:

Google reCAPTCHA

OTP Verification (Email & SMS)

Deployment:

Manual WAR deployment to Apache Tomcat

✨ Key Features
🔐 User Authentication
Role-based login for Candidate and Recruiter

OTP verification (Email/SMS) using JavaMail and Twilio API

Google reCAPTCHA to block bots and spam accounts

👨‍💼 Recruiter Module
Add, edit, or delete job listings

View list of applicants for each job

👨‍💻 Candidate Module
Browse and search jobs by keywords

Apply to jobs with PDF resume uploads

Track applications

📬 Notification System
Email and SMS-based OTP verification

Confirmation messages for key user actions

📊 Performance
REST-style servlets with optimized response time (avg < 200ms)

Designed for concurrent usage (up to 50 users)

99.8% simulated uptime in local testing

🗃️ Database Schema Overview
Table Name	Description
users	Common table for login credentials & role data
candidates	Profile data & uploaded resumes
recruiters	Recruiter profiles & company details
job_posts	Active job listings with metadata
applications	Applied jobs, candidate references

🚀 How to Run (Local Setup)
Clone the Repo

bash
Copy
Edit
git clone https://github.com/your-username/hirehub-jobportal.git
Setup Database

Import schema.sql into MySQL

Update DB credentials in DBUtil.java

Configure APIs

Add your Twilio credentials in OtpSender.java

Update SMTP settings in EmailService.java

Deploy

Package as WAR using your IDE (e.g., Eclipse or IntelliJ)

Deploy to Apache Tomcat 9's webapps/ folder

Access App

Open browser: http://localhost:8080/HireHub/

📚 What I Learned as a Java Full Stack Intern
Practical use of Servlets and session management in Java

Designing modular, secure REST-style services

Real-world integration of third-party APIs (JavaMail, Twilio, Google reCAPTCHA)

Optimizing MySQL queries for concurrent usage

Deploying and testing applications on Apache Tomcat

📌 Future Improvements
Add pagination and filtering to job listings

Admin dashboard to manage platform users

Upgrade to Spring Boot and Thymeleaf for improved scalability
