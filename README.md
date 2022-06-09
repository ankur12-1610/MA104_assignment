## Academic Management System
### Problem:
Candidates are registered in a subject. Once registered, they become students and are assigned a teacher and roll number. Since some students achieve some things throughout the semester, they will be rewarded 10 points in the end. Some students are punished for some reason and are deducted 5 marks. If punished, the achievement grace marks are not added. When results are declared, they are calculated with all things considered. The program displays results.

### Functions of class:
#### Abstract class Registration:
Defines the attributes that are needed for a candidate to register. Contains an abstract method which displays the information.

#### Class Student:
Inherits Registration. Contains additional attributes of professor name and roll number, which are things assigned after registration. Also, the `displayStudent()` method is defined here. A method
`assignProf()` helps to assign a professor based on the subject of student.

#### Class ExamProfile:
Inherits Student class. Contains information if the student is eligible for penalty or grace marks, and
also the test scores of the student. Also, the `showScore()` method displays the score.

#### Interface Achievement:
Contains the marks that are to be rewarded or deducted as grace/penalty.

#### Class Result:
Inherits Examprofile class and implements Achievement. It has a constructor to initiate the class, as well as a method calculatedResult() which calculates the marks based on the conditions. Also, method displayResult() displays the final result of the student.
When a new object is initiated, the constructor assigns the values to the attributes, most of which are inherited from other classes. The method `calculatedResult()` uses control statements to calculate the final marks of the student based on the attributes. The method `displayResult()` uses inherited methods `assignProf()`, `displayStudent()`, `showScore()`, `calculatedResult()` to display the final result.

### Output:

>#### Note:
>For more info visit MA104.pdf
