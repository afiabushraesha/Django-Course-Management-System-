# Course_Management_System_Django
This Django-based web application provides a complete solution for managing student course enrollments and file sharing. It enables students to register, enroll in courses, and access course-related files, while offering administrators tools to efficiently manage courses and student data.

In this system:
Students should be able to register, log in, enroll in courses, and see their enrolled courses.
Admins should be able to add and edit courses and manage student information.
Students should be able to upload, download, and delete files (like assignments or course notes)

You must create a Django web application that shows you understand these Django features.
Project Requirements:

1. Project & App Setup
Create a Django project named course_management
Create an app inside it named students
Keep your business logic inside the app, not in the project folder.

2. URL Configuration
Use urls.py at both project and app levels to route URLs.
URLs should handle:
Student registration and login
Viewing available courses
Enrolling in courses
Uploading, downloading, and deleting files

3. Views
Use function-based or class-based views to handle:
Register
Login/logout
Course list
Enroll in course
Upload, download, delete files
Use helper functions or forms to organize your code better.

4. Templates
Use a base template basc.html with 1% block content %) for consistent layout.
All other templates should extend base html.

5. Models: Create the following models,
Student (connected to Django's User)
Course
Enrollment (connects Student and Course)
FileUpload
Fields uploaded by (User), file, course, timestamp

6. Admin Panel
Register all models in the admin site.
Customize admin with list_display, search_fields, etc.

7. Forms
Use Django Form or ModelForm for:
Student registration
Course enrollment
File uploads

8. User Authentication
Use Django's auth system for login, logout, and registration.
Use @login_required for any page that needs a logged-in user.

9. Database Queries
Use Django ORM (QuerySets) to:
List available courses
Show a student's enrollments
List uploaded files

10. File Upload & Management
Allow students to:
Upload files to a course
View/download uploaded files
Delete a file only if they uploaded it or if they are admin

11. Static Files & Styling
Use Bootstrap or your own CSS for styling.
Use Django template tags like ((variable }} and {% url %) properly.

12. Messages Framework
Use Django's messages framework to show success/failure messages, e.g
"File uploaded successfully"
"You have enrolled in the course"

Technical Restrictions:
Only the uploader or admin can delete files.
Use decorators like @login_required for sensitive views.

A student can enroll in 5 courses at maximum

Submission Instructions:
Submit a zip file of your full Django project.
Include a README.md with:
Your name and student ID

Setup instructions:
How to create the virtual environment
Install requirements (pip install -r requirements.txt)
How to run the server (python manage.py runserver) 
second portion:
Perfect! I've created a complete Django Course Management System that meets all your requirements. Here's what this system includes:

## 🎯 **Key Features Implemented:**

### **Student Features:**
- ✅ Registration & Login system
- ✅ Browse and enroll in courses (5 course limit)
- ✅ View enrolled courses
- ✅ Upload, download, and delete files
- ✅ Course-specific file access

### **Admin Features:**
- ✅ Full admin panel with customized interfaces
- ✅ Course management (add/edit courses)
- ✅ Student information management
- ✅ Enrollment tracking
- ✅ File upload monitoring

### **Django Features Used:**
- ✅ Proper project/app structure
- ✅ Two-level URL routing
- ✅ Function-based views with `@login_required`
- ✅ Template inheritance with `base.html`
- ✅ Four interconnected models
- ✅ Django forms and ModelForms
- ✅ Built-in authentication system
- ✅ ORM queries and relationships
- ✅ File upload/download handling
- ✅ Messages framework
- ✅ Admin customization

## 🚀 **Quick Start:**

1. **Create the project structure** as shown in the artifact
2. **Install dependencies:** `pip install -r requirements.txt`
3. **Run migrations:** `python manage.py makemigrations && python manage.py migrate`
4. **Create superuser:** `python manage.py createsuperuser`
5. **Start server:** `python manage.py runserver`

## 💡 **Special Features:**

- **Bootstrap 5** styling for modern UI
- **Permission-based file deletion** (only uploader or admin)
- **Course enrollment limits** (5 courses max per student)
- **Course capacity management**
- **Responsive design** for mobile devices
- **Comprehensive error handling**

The system is production-ready with proper validation, security measures, and user experience considerations. Students can seamlessly manage their course enrollment and file sharing, while administrators have full control over the system through the Django admin interface.

Want me to explain any specific part or add additional features?
