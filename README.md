# DART-Object-Oriented-Programming
OBJECT Oriented Programmimg challenge
// Student class
class Student {
  String name;
  int age;
  String gradeLevel;

  // Constructor
  Student(this.name, this.age, this.gradeLevel);

  // Method to print student's information
  void printStudentInfo() {
    print('Student: $name, Age: $age, Grade Level: $gradeLevel');
  }
}

// Teacher class
class Teacher {
  String name;
  int age;
  String subject;

  // Constructor
  Teacher(this.name, this.age, this.subject);

  // Method to print teacher's information
  void printTeacherInfo() {
    print('Teacher: $name, Age: $age, Subject: $subject');
  }
}

// Class to create student and teacher objects and call their methods
class School {
  void printInfo() {
    // Create student object
    var student = Student('Alice', 15, '10th');
    // Call method to print student's information
    student.printStudentInfo();

    // Create teacher object
    var teacher = Teacher('Mr. Smith', 35, 'Math');
    // Call method to print teacher's information
    teacher.printTeacherInfo();
  }
}

void main() {
  // Create object of School class
  var school = School();
  // Call method to print student and teacher information
  school.printInfo();
}
