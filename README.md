# CMPS415
All of the projects and works related to the course: Integrated Technologies for Enterprise Systems.

## Homework Assignment 1
Create a class diagram that includes both classes (and the relationship between them) given at the bottom of this assignment. Also, propose another class for Intern by adding it  to your class diagram. The details of this class are entirely up to you.

<hr/>
________________________________________________________________________
public class Employee
{
   private Long id;
   private String firstName;
   private String lastName;

   public Long getId() {
     return id;
   }


   public void setId(Long id) {
     this.id = id;
   }

   public String getFirstName() {
     return firstName;
   }

   public void setFirstName(String firstName) {
     this.firstName = firstName;
   }

   public String getLastName() {
     return lastName;
   }

   public void setLastName(String lastName) {
     this.lastName = lastName;
   }

   public String toString() {
     return "Employee [id=" + id + ", firstName=" + firstName + ",
     lastName=" + lastName + "]";
   }

}

________________________________________________________________________


public class Manager extends Employee
{
   private Employee [] subordinates;

   public Employee [] getSubordinates() {
     return subordinates;
   }

   public void setSubordinates( Employee [] subordinates ) {
     this.subordinates = subordinates;
   }

   public String toString() {
     return "Manager, " + super.toString();
   }
}
