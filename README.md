# SafeRide
1. Introduction

1.1 Purpose
The School Bus Safety System is designed to enhance student safety during transportation. It uses face recognition, GPS tracking, and SMS/WhatsApp notifications to inform parents when their child enters/exits the bus. It also alerts the admin when an unknown person tries to enter.

1.2 Scope
*Face Recognition: Identifies students and logs their entry/exit.
*GPS Tracking: Captures and shares real-time bus location.
*SMS/WhatsApp Notification: Alerts parents about their child’s movement.
*Admin Panel: Manages student registrations, attendance, routes, and alerts.
*Parent Portal: Provides access to bus location and notifications.

1.3 Technologies Used
Frontend: HTML, CSS
Backend: Django
Database: SQLite
APIs: OpenCV (for face recognition), Google Maps API (for GPS), Twilio API (for SMS/WhatsApp)


---


2. Functional Requirements

2.1 User Roles

1. Admin
Register students and manage profiles.
Monitor attendance logs.
Track bus routes and manage alerts.

2. Parents
Receive real-time notifications about student entry/exit.
Access live bus tracking.


2.2 Features
Face Recognition System:
Detect and recognize students entering/exiting.
Store logs in the database.
Trigger notifications to parents.

GPS Tracking System:
Using neo 8m get the tracking.
Display bus location to parents.

Notification System:
Send entry/exit alerts to parents via SMS/WhatsApp.
Alert admin if an unknown person attempts entry.

Admin Panel:
Dashboard for student management, attendance logs, and bus tracking.


---


3. Non-Functional Requirements
Security: Encrypt student data and restrict unauthorized access.
Scalability: Handle multiple buses and students efficiently.
Performance: Fast recognition and notification delivery.


---


4. System Design

4.1 Architecture
Frontend: Displays student data, tracking, and alerts.
Backend: Handles authentication, data processing, and notifications.
Database: Stores student details, logs, and attendance.
APIs: Integrates face recognition, GPS, and notifications.

4.2 Database Schema
Students Table: (ID, Name, Parent Contact, Bus ID, Face Data)
Attendance Table: (Student ID, Time, Location, Status)
Bus Table: (Bus ID, Route, Current Location)
Alerts Table: (ID, Student ID, Time, Alert Type)



---

5. Installation and Deployment

5.1 Prerequisites
Python 3.x
Django
SQLite
OpenCV
Twilio API
Google Maps API

5.2 Setup Steps

1. Clone the Repository
git clone https://github.com/your-repo/SafeRide.git
cd SafeRide

2. Install Dependencies
pip install -r requirements.txt

3. Run Migrations
python manage.py migrate

4. Start the Server
python manage.py runserver

5. Access the Application
Open http://127.0.0.1:8000/ in a browser.
