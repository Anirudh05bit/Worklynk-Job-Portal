# Worklynk-Job-Portal
 Software Requirement Specification (SRS)
Project Title: Job Portal System
 Technologies: React (Frontend), Firebase (Backend)
 Prepared By: Anirudh Suresh
 Date: 22-Aug-2025

1. Introduction
1.1 Purpose
The purpose of this project is to develop a Job Portal System that connects job seekers with employers. The system provides features such as job posting, job search, applications, resume uploads, employer dashboards, and real-time notifications. The backend is powered by Firebase services to ensure scalability, real-time synchronization, and secure authentication.
1.2 Scope
Job Seekers can:


Register/login using Firebase Authentication.


Search and filter jobs.


Apply for jobs by uploading resumes.


Track their applications.


Receive notifications about job updates.


Employers can:


Post jobs with detailed requirements.


View applicants and download resumes.


Manage job postings (edit, delete, close).


Get analytics on job postings.


Admin can:


Manage users (employers, job seekers).


Approve or reject job postings.


Monitor platform activity.


The system will be available as a web application with responsive UI for desktop and mobile.
1.3 Definitions, Acronyms, and Abbreviations
Firebase Auth – Authentication service for user management.


Firestore – Cloud NoSQL database for storing job, user, and application data.


FCM – Firebase Cloud Messaging for push notifications.


CRUD – Create, Read, Update, Delete operations.



2. Overall Description
2.1 Product Perspective
This Job Portal System is a standalone web application built using React for frontend and Firebase for backend services. It integrates Firebase Authentication, Firestore Database, Firebase Storage, and Firebase Cloud Messaging.
2.2 Product Features
User Authentication & Role Management


Google/Email login.


Roles: Job Seeker, Employer, Admin.


Job Posting & Management


Employers can post, edit, delete, and close jobs.


Job seekers can search, filter, and bookmark jobs.


Applications Management


Job seekers can apply with resumes.


Employers can view applicants and manage application statuses.


Notifications & Alerts


Job seekers notified when new jobs are posted.


Applicants notified when their application status changes.


Dashboards


Employer Dashboard: Job posting stats, applicant list.


Job Seeker Dashboard: Applied jobs, saved jobs.


Admin Dashboard: User & job management.


Extras (Future Enhancements)


AI-powered job recommendations.


Resume builder.


Premium job boosting with Stripe payments.


2.3 User Classes and Characteristics
Job Seeker: Basic user, searching for jobs, uploads resumes.


Employer: Posts jobs, manages applicants.


Admin: Manages users and monitors system activity.


2.4 Operating Environment
Frontend: ReactJS


Backend: Firebase (Auth, Firestore, Storage, Cloud Functions, FCM)


Hosting: Firebase Hosting


Supported Devices: Desktop, Tablet, Mobile


2.5 Design and Implementation Constraints
Must use Firebase as backend.


Must support responsive design.


Limited free-tier usage for Firebase (scalability required for production).



3. System Features
3.1 Authentication & Authorization
Secure login via Firebase Auth.


Role-based access control.


3.2 Job Posting
Employers can create jobs with details.


Jobs visible to all job seekers after approval (Admin).


3.3 Job Applications
Job seekers apply with resume upload.


Employers can change application status: Pending, Accepted, Rejected.


3.4 Search & Filters
Search by job title, company, location, salary, skills.


Filter by category and job type (Full-time, Part-time, Remote).


Push notifications for new job postings and application updates.


3.6 Dashboards
Employer Dashboard: Manage jobs & view applicants.


Job Seeker Dashboard: Track applications & saved jobs.


Admin Dashboard: Approve/reject jobs, manage users.





4. External Interface Requirements
User Interface: Responsive React frontend with modern UI (TailwindCSS or Material UI).


Hardware Interface: Standard web browsers (Chrome, Edge, Firefox, Safari).


Software Interface: Firebase APIs, Stripe API (for payments, future).



