# Design Database for GYM system
The Database-for-GYM-system is a comprehensive information management system designed to facilitate the operations of a gym or fitness center. It uses an Entity-Relationship Diagram (ERD) and Schema to organize and store data related to various entities involved in the gym's functioning. Let's describe the entities and their attributes along with the relationships, followed by an overview of what the system can do:

## Entities and their Attributes:

### 1- Equipment:

    Number of equipment
    Equipment ID
    Name
    Target muscles
    Price
### 2- Class:

    Cost
    Class ID
    Class hall
    Opening hour
    Number of trainers
    Max number of trainees
    Number of trainees (current count)
    Closing hour
### 3- Trainer:

    Age
    Trainer ID
    Contact (Phone number, email)
    Salary
    Address
    Social status
    SSN (Social Security Number)
    Birthdate
    Hiring date
    Gender
    Name (First name, last name)
### 4- Trainee:

    Trainee ID
    Name (First name, last name)
    Birthdate
    Body fat percentage
    Age
    Gender
    Body mass index (BMI) (height, weight)
    Contact (Phone number, email)
### 5- Diet:

    Exercises
    Daily meals
    Name
### 6- Membership Type:

    Start date
    End date
    Costs
    Type
### 7- Department:

    Department ID
    Name
    Location
### 8- Employee:

    Age
    Employee ID
    Contact (Phone number, email)
    Salary
    Address
    Social status
    SSN (Social Security Number)
    Birthdate
    Hiring date
    Gender
    Name (First name, last name)
### 9- Sports Tool:

    Price
    Tool ID
    Tool name
    Producing company
    Country of origin
### 10- Food Supplement:

    Supplement ID
    Price
    Product name
    Country of origin
    Date (Production date, expiration date)
## Relationships and Their Descriptions:

### 1- Class uses Equipment (M:N):

  This relationship links classes to the equipment they use and vice versa. It allows tracking which equipment is utilized in different classes and helps ensure that the necessary equipment is available for each class.
### 2- Trainer Trains Class (M:N):
  
  This relationship connects trainers to the classes they train and vice versa. It enables efficient management of trainer assignments to various classes.
### 3- Department Organizes Class (1:M):

This relationship indicates that a department can organize multiple classes, while each class is organized by only one department. It allows the system to manage class organization and assign responsible departments.
### 4- Trainer Instructs Trainee to Class (1:M:N) (Ternary Relationship):

This ternary relationship involves trainers, trainees, and classes. It signifies that a trainer can instruct multiple trainees in specific classes, and a trainee can be instructed by multiple trainers in various classes. It helps in tracking the trainer-trainee-class associations.
### 5- Trainer Gives Trainee Diet (1:1:1) (Ternary Relationship):

This ternary relationship establishes a connection between trainers, trainees, and diet plans. It means that a trainer can provide a diet plan to a specific trainee, and a trainee can receive a diet plan from a particular trainer. It helps personalize diet plans for each trainee.
### 6- Trainee Has Membership Type (N:1):

This relationship links trainees to their respective membership types. It ensures that each trainee is associated with a specific membership type.
### 7- Employee Works for Department (M:1):

This relationship connects employees to the departments they work for. It allows efficient management of employee assignments to different departments.
### 8- Employee Sells Sports Tool (1:M):

This relationship signifies that an employee can sell multiple sports tools. It enables tracking of the sales made by each employee.
### 9- Employee Supplies Food Supplement (1:M):

This relationship indicates that an employee can supply multiple food supplements. It allows the system to track the supply of food supplements made by each employee.
## Capabilities and Functionalities of the System:

The Database-for-GYM-system offers various capabilities and functionalities to streamline gym operations and enhance overall efficiency:

### 1- Class Management:

The system can schedule and manage different fitness classes, including class details, hall allocation, opening, and closing hours.
### 2- Equipment Tracking:

Gym equipment can be tracked, including the number of available items, their identification, names, and target muscles.
### 3- Trainer Management:

The system allows storing and organizing information about fitness trainers, including their qualifications, contact details, and class assignments.
### 4- Trainee Management:

Trainee information, such as personal details, contact information, and fitness-related data (BMI, body fat percentage), can be managed in the system.
### 5- Diet Planning:

Trainers can create personalized diet plans for individual trainees, and trainees can receive and follow their designated diet plans.
### 6- Membership Management:

The system can handle different types of gym memberships, their costs, and duration.
### 7- Department Organization:

The system allows managing different gym departments and associating classes with their respective organizing departments.
### 8- Employee Management:

Employee details, including contact information, salary, and roles within the gym, can be efficiently managed.
### 9- Sales and Supply Management:

The system can track sales of sports tools made by employees and monitor the supply of food supplements provided by employees.
### 10- Reporting and Analysis:

The system can generate various reports, such as class schedules, trainer assignments, membership statistics, and more, to help gym management make data-driven decisions.

#### Overall, the Database-for-GYM-system serves as a powerful tool for gym administrators, trainers, and employees to effectively manage gym operations, enhance member experiences, and optimize the overall fitness center's performance. It facilitates data organization, accessibility, and analysis, contributing to the gym's success and growth.
