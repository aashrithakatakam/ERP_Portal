 # College ERP Practice Project

Small Django project for practicing student, staff, attendance, result, and
administration workflows. It is intended for local learning and experimentation.

## Contents

- [About](#-about)
- [Features](#-features)
- [Demo Credentials](#-demo-credentials)
- [Technology Stack](#-technology-stack)
- [Installation](#-installation)
- [Screenshots](#-screenshots)
- [Roadmap](#-roadmap)

---

## 🎯 About

**College ERP** is a small Django application for learning how common college
administration workflows fit together.

---

## 🚀 Features

### 👨‍💼 Admin Dashboard

<details>
<summary>Click to expand Admin features</summary>

- 📈 **Analytics Dashboard** - Overview charts for student/staff performance, courses, and subjects
- 👥 **Staff Management** - Complete CRUD operations for staff members
- 🎓 **Student Management** - Add, update, and delete student records
- 📚 **Course Management** - Organize and manage academic courses
- 📖 **Subject Management** - Handle subject assignments and details
- 📅 **Session Management** - Control academic sessions and terms
- ✅ **Attendance Monitoring** - View and track student attendance
- 💬 **Feedback System** - Review and respond to feedback from students/staff
- 🏖️ **Leave Management** - Approve or reject leave applications

</details>

### 👨‍🏫 Staff Portal

<details>
<summary>Click to expand Staff features</summary>

- 📊 **Performance Dashboard** - Track student progress and subject analytics
- ✏️ **Attendance Management** - Mark and update student attendance
- 📝 **Result Entry** - Add and modify student examination results
- 🏖️ **Leave Applications** - Apply for personal leave
- 💭 **Feedback Channel** - Send feedback to administration

</details>

### 🎓 Student Portal

<details>
<summary>Click to expand Student features</summary>

- 📊 **Personal Dashboard** - View attendance, results, and leave status
- 📅 **Attendance Tracking** - Monitor class attendance records
- 🎯 **Result Portal** - Access examination results and grades
- 🏖️ **Leave Requests** - Submit leave applications
- 💬 **Feedback System** - Provide feedback to HOD

</details>

---

## 🔑 Demo Credentials

### Login Details

| Role | Email | Password |
|------|-------|----------|
| 👨‍🎓 **Student** | `studentone@student.com` | `studentone` |
| 👨‍🏫 **Staff** | `staffone@staff.com` | `staffone` |

---

## 🛠️ Technology Stack

| Category | Technologies |
|----------|-------------|
| **Backend** | Python, Django Framework |
| **Frontend** | HTML5, CSS3, JavaScript, Bootstrap |
| **Database** | SQLite |
| **Authentication** | Django Auth, Google reCAPTCHA |
| **Use** | Local practice |

---

## 📥 Installation

### Prerequisites

Ensure you have the following installed:

- ✅ [Git](https://git-scm.com/) - Version control
- ✅ [Python 3.x](https://www.python.org/downloads/) - Programming language
- ✅ [pip](https://pip.pypa.io/en/stable/installing/) - Package manager

### Step-by-Step Setup

#### 1️⃣ Open the Project

```bash
cd College-ERP-main
```

#### 2️⃣ Create Virtual Environment

**Option A: Using Conda (Recommended)**
```bash
conda env create -f college-erp.yml
conda activate Django-env
```

**Option B: Using venv**

<details>
<summary>Windows</summary>

```bash
python -m venv venv
source venv/scripts/activate
```
</details>

<details>
<summary>macOS</summary>

```bash
python3 -m venv venv
source venv/bin/activate
```
</details>

<details>
<summary>Linux</summary>

```bash
virtualenv .
source bin/activate
```
</details>

#### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

#### 4️⃣ Configure Settings

Open `settings.py` and update:

```python
ALLOWED_HOSTS = ['localhost', '127.0.0.1']
```

> ⚠️ **Security Note:** Never use `ALLOWED_HOSTS = ['*']` in production!

#### 5️⃣ Database Setup

```bash
python manage.py migrate
python manage.py createsuperuser
```

Follow the prompts to create an admin account.

#### 6️⃣ Run Development Server

```bash
# Windows
python manage.py runserver

# macOS/Linux
python3 manage.py runserver
```

🎉 **Success!** Visit `http://127.0.0.1:8000` in your browser

---

## 📸 Screenshots

![Demo Screenshot](Showcase/Screenshot_04.png)
![Demo Screenshot](Showcase/Screenshot_03.png)
![Demo Screenshot](Showcase/Screenshot_01.png)
![Demo Screenshot](Showcase/Screenshot_02.png)


---

## 🗺️ Roadmap

### ✅ Completed Features

- [x] Multi-role authentication system
- [x] Complete CRUD operations for all entities
- [x] Attendance management system
- [x] Result management with CBVs
- [x] Leave application workflow
- [x] Feedback system
- [x] Email notifications
- [x] Google reCAPTCHA integration
- [x] Profile management for all roles
- [x] Dynamic dashboard analytics
- [x] Responsive design
- [x] Password reset functionality

### 🔜 Upcoming Features


- [ ] SMS notifications
- [ ] Advanced reporting and analytics
- [ ] Online examination module
- [ ] Library management system
- [ ] Fee management integration
- [ ] Timetable generator
- [ ] Parent portal

---

## Practice Notes

This project uses SQLite and local settings so it can be run and changed while
learning Django. Update the settings and demo data as needed for your own
practice.