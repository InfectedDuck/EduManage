# Online Course Management System

A Django-based web application designed for managing online courses, user registrations, and exam submissions. This project showcases robust backend development, user authentication, and dynamic content handling using Django.

## Features

- **User Authentication**: Register, log in, and log out users with session management.
- **Course Management**: Browse courses, view detailed information, and enroll in courses.
- **Enrollment Tracking**: Track user enrollments and manage course participation.
- **Exam Submissions**: Submit exam answers and view results with grading.
- **Dynamic Content**: Manage course content, questions, and user data using Django's ORM.

## Key Features

- **Full CRUD Operations**: Create, Read, Update, and Delete operations for courses, lessons, and enrollments.
- **User Roles**: Differentiates between instructors and learners with specific attributes and roles.
- **Course Enrollment**: Manage enrollments with support for various course modes (Audit, Honor, Beta).
- **Automated Testing**: Ensure robust functionality with Django's built-in testing framework.
- **Dynamic Exam Handling**: Submit answers and get results based on user submissions.

## Tech Stack

- **Django**: Web framework for developing the application.
- **SQLite**: Default database for storing course and user data.
- **Bootstrap**: Frontend framework for responsive design.
- **Logging**: Integrated logging for tracking errors and application events.

## Models

- **Instructor**: Represents course instructors with attributes such as user, full-time status, and total learners.
- **Learner**: Represents course learners with attributes like occupation and social link.
- **Course**: Represents courses with attributes like name, description, image, and instructors.
- **Lesson**: Represents lessons within a course.
- **Enrollment**: Tracks user enrollments in courses with attributes like enrollment date, mode, and rating.
- **Question**: Represents exam questions with associated grades.
- **Choice**: Represents choices for questions with correct/incorrect status.
- **Submission**: Tracks user submissions with chosen answers.

## Views

- **CourseListView**: Displays a list of courses with enrollment status.
- **CourseDetailView**: Shows detailed information about a specific course.
- **Enroll**: Handles course enrollment for authenticated users.
- **Submit**: Manages exam submissions and redirects to result view.
- **Show Exam Result**: Displays the results of an exam submission.

## URLs

- `/`: Home page with a list of courses.
- `/registration/`: User registration page.
- `/login/`: User login page.
- `/logout/`: User logout.
- `/course/<int:pk>/`: Course detail page.
- `/course/<int:course_id>/enroll/`: Enroll in a course.
- `/course/<int:course_id>/submit/`: Submit exam answers.
- `/course/<int:course_id>/submission/<int:submission_id>/result/`: View exam results.


# **General Notes**

An `onlinecourse` app has already been provided in this repo upon which you will be adding a new assesement feature.

- If you want to develop the final project on Theia hosted by [IBM Developer Skills Network](https://labs.cognitiveclass.ai/), you will need to create the same project structure on Theia workspace and save it everytime you close the browser
- Or you could develop the final project locally by setting up your own Python runtime and IDE
- Hints for the final project are left on source code files
- You may choose any cloud platform for deployment (default is IBM Cloud Foundry)
- Depends on your deployment, you may choose any SQL database Django supported such as SQLite3, PostgreSQL, and MySQL (default is SQLite3)

**ER Diagram**
For your reference, we have prepared the ER diagram design for the new assesement feature.

![Onlinecourse ER Diagram](https://github.com/ibm-developer-skills-network/final-cloud-app-with-database/blob/master/static/media/course_images/onlinecourse_app_er.png)


## License
This project is licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for details. <br>
This project is made as a part of IBM Course.
