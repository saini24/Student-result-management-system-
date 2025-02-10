# Student-result-management-system-
In the Student Result Management System code, several fundamental coding skills are used. Here's a breakdown of the key skills:

1. Object-Oriented Programming (OOP)
Classes and Objects: The code uses classes (Student and ResultManagementSystem) to represent entities (students and the result management system). OOP concepts like encapsulation (storing data within objects) and abstraction (hiding complex logic within methods) are applied.
Methods: Functions defined inside classes, such as add_student(), display_result(), and calculate_grade(), perform specific actions related to those objects.
Attributes: The Student class has attributes like student_id, name, and subject_marks, while the ResultManagementSystem class stores a list of student objects (self.students).
2. Functions and Methodology
Defining Functions: The program defines multiple functions (add_student(), display_result(), search_student(), etc.) to handle specific tasks.
Parameter Passing: Functions take inputs (e.g., student_id, name, subject_marks) and return results (e.g., displaying student information).
3. Loops
For Loops: Used in the code to iterate over subjects and collect marks, e.g., in add_student():
python
Copy
Edit
for i in range(num_subjects):
    mark = float(input(f"Enter marks for subject {i + 1}: "))
    subject_marks.append(mark)
While Loop: The run() method uses a while True loop to repeatedly show the main menu and handle user input until the user decides to exit.
4. Conditional Statements
If-Else Statements: Used for decision-making, such as calculating the grade based on the average marks in the calculate_grade() method:
python
Copy
Edit
if self.average >= 90:
    return 'A+'
elif self.average >= 80:
    return 'A'
These statements are also used to navigate through different menu options and perform appropriate actions.
5. Input and Output Handling
Taking User Input: The program uses input() to gather information from the user (e.g., student details, subject marks).
Displaying Output: The print() function is used extensively to display results, menus, and error messages.
6. Data Structures
Lists: The subject_marks list stores the marks for each student, and the students list stores the objects of all students.
String Operations: String manipulation is used to format the student results and create clear, readable output.
7. Error Handling (Optional but important for further enhancement)
Type Conversion: Handling user input and converting it to the appropriate type (float for marks).
You might also add checks for invalid data (e.g., non-numeric input) to make the program more robust.
8. Modularization
Separation of Concerns: The code is structured in a modular way, with each class and method handling specific tasks. This helps with readability and maintainability.
9. Basic Algorithmic Thinking
Grade Calculation: The calculate_grade() method is a simple algorithm based on conditional checks.
Average Calculation: The average is calculated by summing the marks and dividing by the number of subjects.
10. File Handling (Extension Possibility)
Although the current version does not include file handling, saving student data to a file (e.g., using pickle or json) could be a natural extension of this project.
