# CAR-MEMBERSHIP-SYSTEM
# Car Membership App

Welcome to the Car Membership App! This application is designed to manage car parking memberships, allowing users to sign up, search for members, and providing administrative controls for managing memberships. It provides a user-friendly interface powered by Java Swing and is integrated with a MySQL database to store membership information.

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [System Requirements](#system-requirements)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Database Schema](#database-schema)
7. [App Screenshots](#app-screenshots)
8. [License](#license)

## Introduction

The Car Membership App allows users to:
- Register for membership by providing their personal details and car information.
- View, search, and manage existing memberships.
- Administrators can add new members, search by license plate, and view all registered members.

This app uses **Java Swing** for the GUI and **MySQL** for storing member data. It offers functionalities for both **Users** and **Admins**.

## Features

- **User Interface:**
  - Login screen for users to select their role (User or Admin).
  - Search members by name, car model, or license plate.
  - Easy-to-use and responsive GUI for efficient navigation.
  
- **Admin Interface:**
  - Admins can add new members with details like name, car model, license plate, membership type, contact, and payment method.
  - Admins can view all registered members.
  - Admins can search members by license plate.

- **Database Integration:**
  - MySQL database stores user information, car models, membership types, and payment details.
  - CRUD (Create, Read, Update, Delete) operations on members.

## System Requirements

Before running the Car Membership App, ensure your system meets the following requirements:

| Requirement         | Details                                 |
|---------------------|-----------------------------------------|
| **Java Version**     | Java 8 or later                         |
| **MySQL Database**   | MySQL 5.7 or later                      |
| **IDE**              | IntelliJ IDEA, NetBeans , or similar Java IDE |
| **Libraries**        | JDBC for database connectivity, Swing for GUI |

## Installation

To get started with the Car Membership App, follow these installation steps:

### 1. Clone the repository:
```bash
git clone https://github.com/haseeb0033/car-membership-app.git
cd car-membership-app
```


### 2. Set up MySQL Database:
1. Install MySQL on your local machine or use a remote MySQL server.
   
2. Create a new database named car_membership.
   
3. Create a table for storing member information. You can use the following SQL script:

```sql
CREATE TABLE members (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    car_model VARCHAR(50),
    license_plate VARCHAR(20),
    membership_type VARCHAR(20),
    contact VARCHAR(50),
    account_number VARCHAR(50)
);
```

### 3. Update Database Credentials:
- In the CarMembershipApp.java file, update the database connection string with your credentials:

```java
private static final String DB_URL = "jdbc:mysql://localhost:3306/car_membership";
private static final String DB_USER = "localhost";
private static final String DB_PASS = "12345";
```

### 4. Compile and Run the Application:
1. Open the project in your preferred Java IDE.
2. Compile and run the CarMembershipApp.java file.
## Usage
Once the application is up and running, you can follow these steps:

- Launch the Application: Start the application to see the welcome screen.
- Login: Choose between the User and Admin role.
## User Interface:
- Select a search option (Name, Car Model, License Plate).
- Enter the value and click Search to find members.
## Admin Interface:
- Add new members by filling out the provided form with car and membership details.
- View all registered members.
- Search members by license plate.
## Example Usage:
1. User Login: Select "User" to search for a car by name, model, or license plate.
2. Admin Login: Select "Admin" to add new members, view the list of all members, or search for a member by license plate.

### 5. Database Schema

The **members** table in the database consists of the following columns:

| Column Name        | Data Type    | Description                                       |
|--------------------|--------------|---------------------------------------------------|
| `id`               | INT          | Primary Key, Auto Increment                       |
| `name`             | VARCHAR(100) | Member's name                                     |
| `car_model`        | VARCHAR(50)  | Car model                                         |
| `license_plate`    | VARCHAR(20)  | Car license plate                                 |
| `membership_type`  | VARCHAR(20)  | Membership type (Basic, Premium, VIP)             |
| `contact`          | VARCHAR(50)  | Member's contact details                          |
| `account_number`   | VARCHAR(50)  | Payment method account number                     |

## App Screenshots
- Here are some screenshots of the app in action:

**Welcome Page :** 




![1](https://github.com/user-attachments/assets/62e1aded-5cc9-456a-9698-fbb83f64275f)





**Login Page**


![2](https://github.com/user-attachments/assets/e5e57897-fb4e-479d-8d11-194553eb2064)



**User Search Page**




![3](https://github.com/user-attachments/assets/1f7ed5e2-c229-4891-997d-e5325856a886)






**Admin Dashboard**





![4](https://github.com/user-attachments/assets/ccc2a6fd-c5d6-4dc5-ab1a-1f28a9cff642)





## License
This project is licensed under the MIT License - see the LICENSE file for details.

- Feel free to contribute, report bugs, or suggest features by opening an issue or a pull request.
- Thank you for using the Car Membership App!


### Explanation:

1. **Table of Contents**: Provides an easy-to-navigate list of sections in the README.
2. **Introduction**: Explains what the app is and what it does.
3. **Features**: Describes key functionalities of the app.
4. **System Requirements**: Specifies what is needed to run the project.
5. **Installation**: Provides clear instructions to set up and run the app locally.
6. **Usage**: Describes how to interact with the application once it is running.
7. **Database Schema**: Shows the structure of the database table used to store member data.
8. **App Screenshots**: Visual representation of the app’s UI (you can upload screenshots to an `assets/screenshots/` folder on your GitHub repo).
9. **License**: Standard license section, assuming MIT License.





