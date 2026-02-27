# Academic Information System (IAS) – Legacy Version
This repository contains a legacy Academic Information System used internally by the institution since 2018.
The system manages student profiles, course catalog, enrollment records, and grading.

## System Overview
The IAS is composed of four internal subsystems:

- Student Profile Management
- Course Management
- Enrollment Record Management
- Grading System

### Student Profile Management
Responsible for maintaining student identity records.

Core Functions:
- Create Student
- View All Students
- View Student by ID

Note:
Student ID is randomly generated strings.

### Course Management
Maintains course catalog information.

Core Functions:
- Create Course
- View Courses

### Enrollment Record Management
Handles student course enrollments per academic term.

### Grading System
Stores final grades submitted by instructors.

Core Functions:
- Create Grade
- View All Grades
- View Grades by Student ID

Core Functions:
- Add Enrolled Course by Student ID
- View Enrollment by Student ID
- View All Enrollments

## Data Considerations
- Each module maintains its own data model.
- No global schema enforcement exists across modules.
- Identifier formats may vary.
- Term naming conventions are not standardized.
- Cross-module validation is limited.

## API Overview

Each subsystem exposes REST-like endpoints.
- Student profile management
``` Bash
GET /api/students
GET /api/students/{id}
POST /students
```

- Course management
``` Bash
GET /api/courses
POST /api/courses
```

- Enrollment record management
``` Bash
GET /api/enrollments
GET /api/enrollments/{studentId}
POST /enrollments
```

- Grading system
``` Bash
GET /api/grades
GET /api/grades/{studentId}
POST /api/grades
```

## Academic Exercise Context

This system is intentionally designed to simulate a legacy environment.

Students are expected to:
- Analyze system boundaries
- Identify inconsistencies
- Propose integration strategies
- Recommend modernization approaches

Check the system [here](https://ais-simulated-legacy.onrender.com/api/students) for more information.

