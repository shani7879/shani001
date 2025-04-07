
// Base Class: Person
class Person {
    String name;
    int age;

    void displayPersonInfo() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}

// Single Inheritance: Employee inherits from Person
class Employee extends Person {
    String employeeId;
    String department;

    void displayEmployeeInfo() {
        displayPersonInfo();  // Call Person method
        System.out.println("Employee ID: " + employeeId);
        System.out.println("Department: " + department);
    }
}

// Multilevel Inheritance: Manager inherits from Employee
class Manager extends Employee {
    int teamSize;

    void displayManagerInfo() {
        displayEmployeeInfo();  // Call Employee method
        System.out.println("Team Size: " + teamSize);
    }
}

// Main class to run the program
public class InheritanceDemo {
    public static void main(String[] args) {
        // Create a Manager object