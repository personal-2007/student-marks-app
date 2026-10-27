# Student Marks Calculator using Java Servlet and JSP

A simple web-based application that accepts a student's name and marks in three subjects, validates the marks, and displays the total marks, average marks, and final grade on a separate result page.

## Features

- Enter the student's name.
- Enter marks for three subjects.
- Validate marks between 0 and 100.
- Calculate total marks out of 300.
- Calculate average marks.
- Display the final grade.
- Show the result on a separate page.
- Navigate back to the input form.

## Technologies Used

- Java
- Jakarta Servlet
- JSP (JavaServer Pages)
- HTML
- Maven
- Apache Tomcat 10.1
- Eclipse IDE

## Application Screenshots

### 1. Student Marks Input Form

The input page allows students to enter their name and marks for three subjects.

![Student Marks Input Form](screenshots/student-marks-form.png)

### 2. Student Result Page

The result page displays the student's name, total marks, average marks, and final grade.

**Sample Output:**

- **Student Name:** SELVAKUMAR S
- **Total Marks:** 240 / 300
- **Average Marks:** 80.00
- **Final Grade:** B

![Student Result Page](screenshots/student-marks-result.png)

## Grade Criteria

The following is an example grading system. Ensure that it matches the grade criteria implemented in `MarksServlet.java`.

| Average Marks | Grade |
|---|---|
| 90–100 | A |
| 75–89.99 | B |
| 60–74.99 | C |
| 50–59.99 | D |
| Below 50 | F |

## How to Run the Project

1. Install JDK 21, Eclipse IDE for Enterprise Java and Web Developers, and Apache Tomcat 10.1.
2. Import the project into Eclipse as an existing Maven project.
3. Configure the project with WAR packaging and the Jakarta Servlet API dependency.
4. Add Tomcat 10.1 to Eclipse.
5. Right-click the project and select **Run As → Run on Server**.
6. Open the application in your browser:

   `http://localhost:8080/student-marks-app/`

## Project Structure

```text
student-marks-app/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/example/marks/
│       │       └── MarksServlet.java
│       └── webapp/
│           ├── index.jsp
│           └── result.jsp
├── pom.xml
└── README.md
```

## Input Validation

Each subject mark must be a valid number between 0 and 100. Invalid or missing inputs should be rejected with an appropriate error message.

## Author

**SELVAKUMAR S**

## Purpose

This project was developed for educational purposes to demonstrate Java Servlet, JSP, form handling, input validation, calculations, and result presentation in a web application.
