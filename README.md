package oopprojects;

public class Main {

    public static void main(String[] args) {

        System.out.println("Java OOP Test Projects Repository");
        System.out.println("Core and Advanced OOP concepts implemented");
        System.out.println("Each concept as separate project under src directory");

        Person p = new Person("Ashik", 22);
        p.displayInfo();

        Circle c = new Circle(7);
        System.out.println("Circle area: " + c.calculateArea());

        Employee e = new Employee("Rahim", "CSE", 50000);
        e.displayEmployee();
    }
}

class Person {
    private String name;
    private int age;

    Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public void displayInfo() {
        System.out.println("Name: " + name + ", Age: " + age);
    }
}

class Circle {
    private double radius;

    Circle(double radius) {
        this.radius = radius;
    }

    public double calculateArea() {
        return Math.PI * radius * radius;
    }
}

class Employee {
    private String name;
    private String department;
    private double salary;

    Employee(String name, String department, double salary) {
        this.name = name;
        this.department = department;
        this.salary = salary;
    }

    public void displayEmployee() {
        System.out.println("Employee: " + name + ", Dept: " + department + ", Salary: " + salary);
    }
}
