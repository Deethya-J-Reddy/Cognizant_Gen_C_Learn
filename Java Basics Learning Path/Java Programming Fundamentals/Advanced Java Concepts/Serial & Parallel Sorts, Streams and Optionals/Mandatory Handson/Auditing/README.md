# Auditing

Lego is a famous company in the city. The company is due for auditing in the upcoming days. During the auditing details of the employees will be verified, but only for selected employees.  Manually collecting the details will be difficult. So help them to print the details of the employees as per the requirement. The details of the employees need to be printed according to their salary.

Help them to write a java program to find the employees whose salary is less than or equal to the salary specified by the auditors using Lambdas.

## Requirement 1:

Find the employee details

Lego company wants to identify the employees whose salary is less than or equal to the salary specified by the auditors. By using the method fetchEmployeeDetails, identify the employees whose salary is less than or equal to the salary specified by the auditors.

### Component Specification: Employee Interface- This is a Functional Interface.

| Type(Interface) | Methods | Responsibilities | 
| --------------- | ------- | ---------------- |
| EmployeeAudit | `public ArrayList<String> fetchEmployeeDetails(double salary)` | This method is used to identify the employees whose salary is less than or equal to the salary passed as an argument by using Lambda expressions. |
 

### Component Specification: Main Class

- Add the employee details using a Map which holds the key as Employee name and value as Employeesâ€™ salary. Where the map is given as a private attribute with the getters and setters as a part of the code skeleton.
- Then implement the method public static EmployeeAudit findEmployee() which holds the employee details using Lambda Expressions.

| Component Name | Type(Class) | Methods | Responsibilities |
| -------------- | ----------- | ------- | ---------------- |
| Obtain Employee Details | Main | `public void addEmployeeDetails(String employeeName, double salary)` | This method is used to add the employee details into a map. |
| Obtain Employee Details | Main | `public static EmployeeAudit findEmployee()` | This method should return an EmployeeAudit object. To do this, implement the Lambda expression and identify the employees whose salary is less than or equal to the salary passed as an argument. |

If the returned list is empty, then display **â€śNo Employee Foundâ€ś**.

Use appropriate collections to perform the above tasks.

In the Main class create a Main method with the menu as described in the sample Input and Output. 

1. When the user selects option **1** Add Employee details, add the employeeName and salary to the employeeMap.
2. When the user selects option **2** Find Employee details, it should display the employee name returned by the findEmployee method of Main class. If no employee is present, then it should display â€ť No Employee Foundâ€ś.
3. When the user selects option **3** Exit, display the message "Letâ€™s complete the session" and terminate the program.

**Donâ€™t create an object for EmployeeAudit. Use the lambda expression.**

In the Main class write the Main method and perform the given steps :

- Get the details of the Employees.
- Invoke the static method in the Main to identify whose salary is less than or equal to the salary specified
- Capture the object of EmployeeAudit returned by the static method.
- Display the result as shown in the sample output.

> Sample Input and Output:

    1.Add Employee Details
    2.Find Employee Details
    3.Exit
    Enter the choice
    1
    Enter the Employee name
    Faruq
    Enter the Employee Salary
    10000
    1.Add Employee Details
    2.Find Employee Details
    3.Exit
    Enter the choice
    1
    Enter the Employee name
    Benny
    Enter the Employee Salary
    20000
    1.Add Employee Details
    2.Find Employee Details
    3.Exit
    Enter the choice
    2
    Enter the salary to be searched
    15000
    Employee List
    Faruq
    1.Add Employee Details
    2.Find Employee Details
    3.Exit
    Enter the choice
    3
    Let's complete the session