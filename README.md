# 📚 Course Management System with Django

This Django-based web application provides a complete solution for managing student course enrollments and file sharing. It enables students to register, enroll in courses, and access course-related files, while offering administrators tools to efficiently manage courses and student data.

---

## 🔑 System Overview
- 👩‍🎓 **Students** can:
  - Register, log in, enroll in courses, and view enrolled courses
  - Upload, download, and delete files (assignments, notes, etc.)

- 👨‍💼 **Admins** can:
  - Add and edit courses
  - Manage student information
  - Monitor uploaded files

---

## 🛠 Project Requirements

### 1. Project & App Setup
- Create a Django project named **`course_management`**
- Create an app named **`students`**
- Keep all business logic inside the app

### 2. URL Configuration
- Use `urls.py` at both project and app levels
- URLs should handle:
  - Student registration & login
  - Viewing available courses
  - Enrolling in courses
  - File upload, download, and deletion

### 3. Views
- Register / Login / Logout
- Course list & enrollment
- File upload, download, delete
- Use helper functions or forms for cleaner code

### 4. Templates
- Use a base template `base.html` with `{% block content %}`
- Extend `base.html` in all other templates

### 5. Models
- **Student** (linked to Django’s User)
- **Course**
- **Enrollment** (connects Student and Course)
- **FileUpload** (uploaded_by, file, course, timestamp)

### 6. Admin Panel
- Register all models in the admin site
- Customize with `list_display`, `search_fields`, etc.

### 7. Forms
- Student registration
- Course enrollment
- File uploads (via Django Form or ModelForm)

### 8. Authentication
- Use Django’s built-in `auth` system
- Protect views with `@login_required`

### 9. Database Queries
- List available courses
- Show student’s enrollments
- List uploaded files

### 10. File Upload & Management
- Students can upload/download files
- Only the uploader or admin can delete files

### 11. Static Files & Styling
- Bootstrap or custom CSS
- Use template tags (`{{ variable }}` and `{% url %}`)

### 12. Messages Framework
- Show success/failure messages, e.g.:
  - *“File uploaded successfully”*
  - *“You have enrolled in the course”*

---

## ⚙️ Technical Restrictions
- A student can enroll in **maximum 5 courses**
- Only uploader/admin can delete files
- Use decorators like `@login_required` for secure views

---

## 📦 Submission Instructions
- Submit a **zip file** of the full Django project
- Include a **README.md** with:
  - Your name & student ID
- Setup instructions:
  ```bash
  # Create virtual environment
  python -m venv venv
  source venv/bin/activate   # (Linux/Mac)
  venv\Scripts\activate      # (Windows)

  # Install requirements
  pip install -r requirements.txt

  # Run server
  python manage.py runserver
