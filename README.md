# SafeRide – A Smart School Bus Safety System Using Edge Computing

SafeRide is an AI-powered, real-time school bus monitoring system that ensures the **safety and security of students** during their transportation. The system uses **face recognition**, **GPS tracking**, and **automated notifications** to keep parents and administrators informed — all in real-time.

---

## 1. Introduction

### 1.1 Purpose
SafeRide enhances school transport safety by:
- Recognizing students through face recognition
- Sending real-time SMS/WhatsApp alerts to parents
- Alerting the admin in case of unauthorized entry

### 1.2 Scope
- **Face Recognition:** Track student entry/exit using facial biometrics  
- **GPS Tracking:** Live tracking of school bus location  
- **SMS/WhatsApp Notifications:** Instant alerts to parents  
- **Admin Panel:** Manage students, attendance, routes, and alerts  
- **Parent Portal:** Monitor bus location and receive notifications  

### 1.3 Technologies Used

| Component  | Technology |
|------------|------------|
| Frontend   | HTML, CSS  |
| Backend    | Django     |
| Database   | SQLite     |
| Face Recognition | OpenCV |
| GPS        | Neo 8M GPS + Google Maps API |
| Messaging  | Twilio API for SMS & WhatsApp |

---

## 2. Functional Requirements

### 2.1 User Roles

**Admin**
- Register students
- Monitor attendance and bus movement
- Receive alerts on stranger detection

**Parents**
- Receive entry/exit notifications
- View live bus location

### 2.2 Core Features

- **Face Recognition:**  
  Detects and logs student presence using face data

- **GPS Tracking:**  
  Live tracking via Neo 8M module integrated with Google Maps

- **Notifications:**  
  Instant SMS alerts to parents and admin

- **Admin Panel:**  
  Dashboard for managing data and monitoring attendance

---

## 3. Installation & Deployment

### 3.1 Prerequisites

* Python 3.x
* Django
* SQLite
* OpenCV
* Twilio API
* Google Maps API

### 3.2 Setup Steps

```bash
# 1. Clone the repository
git clone https://github.com/uahm/SafeRide.git
cd SafeRide

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run migrations
python manage.py migrate

# 4. Start the server
python manage.py runserver
```

👉 Open your browser and go to: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

---

## 4. Screenshots

### Home Page

![Home](https://github.com/user-attachments/assets/8564da70-bb79-499e-b6b3-55a831f5fdb3)

### Key Features

![Features](https://github.com/user-attachments/assets/5d0296bb-b865-4ac8-ad3a-6cd2b2a4dfd7)

### Adding Student

![Add Student](https://github.com/user-attachments/assets/4dd5f830-b515-4a1b-bcb0-e3411fef5a92)

### Admin Login

![Login](https://github.com/user-attachments/assets/62ef908b-ea9f-4b94-97eb-9a1b60592c10)

### Admin Dashboard

![Dashboard](https://github.com/user-attachments/assets/0bbe17ea-6a34-4f5e-a492-31af69f462f1)

### Attendance Page

![Attendance](https://github.com/user-attachments/assets/32b6ecf6-3935-4cab-b5d0-2201ef296e88)

### Parent Login

![Parent](https://github.com/user-attachments/assets/5ed81756-354d-4187-8609-9594e8761311)

### Live Bus Tracking

![Map](https://github.com/user-attachments/assets/60270917-5429-499b-8300-80a8c90a0429)

---

> 🎓 *This project was built as a final year project to address school transport safety using real-time computer vision, IoT, and communication tools.*
