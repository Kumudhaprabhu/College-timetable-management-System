# Timetable Management System - Project Requirements

## 1. Overview
A web-based timetable management system for departments to create, manage, and view academic timetables efficiently. The system should support department administrators, faculty, and optionally students with role-based access and automated conflict detection.

## 2. Core Functional Requirements

### 2.1 User Authentication
- Secure login and logout
- Role-based access for:
  - Department Admin
  - Faculty
  - Students (optional)
- Password reset functionality

### 2.2 Department Management
- Add, edit, and delete departments
- Manage academic years
- Manage semesters
- Manage sections

### 2.3 Faculty Management
- Add faculty details
- Assign subjects to faculty
- Faculty workload calculation
- Availability preferences
- Leave management

### 2.4 Subject Management
- Add, edit, and delete subjects
- Subject code and credits
- Theory/Lab classification
- Elective subject support

### 2.5 Classroom Management
- Add classrooms
- Lab management
- Capacity tracking
- Room type classification (Lecture/Lab)

### 2.6 Timetable Generation
- Manual timetable creation
- Automatic timetable generation
- Drag-and-drop timetable editor
- Conflict detection for:
  - Faculty clash
  - Room clash
  - Section clash
  - Fixed slots for labs

### 2.7 Timetable View
- Department timetable
- Faculty timetable
- Classroom timetable
- Student timetable
- Weekly and daily views

### 2.8 Notifications
- Notify faculty about timetable changes
- Email notifications (optional)
- Dashboard announcements

### 2.9 Leave & Substitute Management
- Faculty applies for leave
- Suggest substitute faculty
- Temporary timetable adjustment

### 2.10 Attendance Integration (Optional)
- Attendance based on timetable
- Quick attendance marking
- Attendance reports

### 2.11 Search & Filters
- Search by faculty, subject, classroom, or section
- Filter by semester/year

### 2.12 Reports
- Faculty workload report
- Classroom utilization report
- Subject allocation report
- Timetable PDF export
- Excel export

### 2.13 Dashboard
- Today’s classes
- Upcoming classes
- Free classrooms
- Faculty workload summary
- Recent timetable changes

### 2.14 Calendar Integration
- Academic calendar
- Holidays
- Exam schedules
- Event scheduling

## 3. Conflict Detection Rules
The system should automatically detect:
- Same faculty assigned to two classes at the same time
- Same classroom booked twice
- Same section assigned multiple classes at once
- Exceeding faculty workload limits

## 4. Audit & History
- Track who changed the timetable
- Maintain change history
- Restore previous versions

## 5. File Import/Export
- Import faculty from Excel/CSV
- Import subjects
- Export timetable to:
  - PDF
  - Excel
  - CSV

## 6. User Experience Requirements
- Mobile-friendly responsive UI
- Timetable optimized for phones
- Dark mode support

## 7. Suggested Tech Stack

### Frontend
- HTML
- CSS
- Bootstrap
- JavaScript

### Backend
- Node.js
- Express.js

### Database
- MySQL

### Authentication
- JWT
- bcrypt

### Optional Tools
- Sequelize
- pdfkit
- exceljs
- Chart.js

## 8. Team Division

### Member 1 – Frontend + UI
- UI design
- Dashboard
- Forms
- Timetable UI
- Drag-and-drop
- Responsive design
- Dark mode

### Member 2 – Backend + Database
- Database design
- APIs
- Authentication
- Timetable logic
- Conflict detection
- Reports
- Export features