# Object-Oriented Programming Homework 3

This project is part of my Object-Oriented Programming course homework, and it involves creating an application for generating transcripts of students. The project consists of several classes, each with specific functionalities. Below is an overview of the project structure and the classes involved.

## Project Structure

The project is organized into two packages:

1. `hw3.util`: Contains utility classes used in the application.
2. `hw3.main`: Contains the main classes responsible for generating transcripts.

## Classes and Functionalities

### Package `hw3.util`

#### Enum Grade

- The `Grade` enum type represents the grade of a student and defines constants for grades A, B, C, D, and F.
- Each constant is named `Grade.A`, `Grade.B`, `Grade.C`, `Grade.D`, and `Grade.F`.
- The `Grade` enum has two instance fields: `stringValue` (String representation of the letter grade) and `numericValue` (numeric grade corresponding to the letter grade).
- The `toString()` method of `Grade` displays the letter and numerical grade stored for a grade.

#### GradeTest

- The `GradeTest` class is a test program for the `Grade` enum.
- It uses the enhanced for loop and the `values()` method of `Grade` to print out the grade details.

### Package `hw3.main`

#### CourseGrade

- The `CourseGrade` class stores information about a course, including the department, course code, credit, and grade taken.
- The department is a four-letter acronym (CENG, COMP, ECE, ME, MATH).
- The course code is a three-digit number between 100 and 599.
- The course credit can be 3 or 4.
- The grade taken is represented by the `Grade` enum.
- The class provides getters and setters for the fields, with argument validation and default values as specified in the requirements.
- The `setGradeTaken` method is overloaded to handle both double values and `Grade` objects.
- There are four constructors to handle different input combinations and set the default values.
- The constructors use the set methods to set the fields.
- The `toString()` method of `CourseGrade` displays all the information for a course.

#### Transcript

- The `Transcript` class represents the transcript of a student, containing the student's ID and an arbitrary number of `CourseGrade` objects.
- The class also calculates and stores the GPA of the student as a double field (average of all grades taken by the student).
- The one-argument constructor sets the student's ID, initializes the GPA to 0.0, and initializes the list of `CourseGrade` objects.
- The `addCourseTaken` method adds a `CourseGrade` object to the transcript list and updates the GPA accordingly.
- The `toString()` method of `Transcript` displays the student's transcript along with the GPA.

## Getting Started

To use this project, follow these steps:

1. Clone the repository to your local machine.
2. Open the project in your preferred Java IDE (e.g., IntelliJ IDEA).
3. Explore the different packages and classes to understand their functionalities.
4. You can use the provided `GradeTest` class to verify the correctness of the `Grade` enum.
5. Create instances of `CourseGrade` and `Transcript` to generate and display transcripts for different students.

