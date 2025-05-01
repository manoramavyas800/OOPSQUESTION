# OOPSQUESTION
/*Define a class Employee with private attributes (like name, age,
and salary), public methods to get and set these attributes, and a
package-private method to displayEmployeeDetails. Create
another class in the same package to test access to the
displayEmployeeDetails method.*/
package Employees;
public class Employees {
    private String name;
    private int salary;
    public int age;
    public Employees(String name, int salary , int age) {
        this.name = name;
        this.salary = salary;
        this.age = age;
    }
    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public int getSalary() {
        return salary;
    }
    public void setSalary(int salary) {
        this.salary = salary;
    }
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }
    void displayEmployeedetails() {
        System.out.println("Name: " + name+" "+"age: "+ age+" "+"salary: " + salary);
    }



    package Employees;

public class EmployeeTest {
    public static void main(String[] args) {
        Employees emp=new Employees("Mahi",50000,18);
        emp.displayEmployeedetails();

    }
}
