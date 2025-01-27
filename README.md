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
| **IDE**              | IntelliJ IDEA, Eclipse, or similar Java IDE |
| **Libraries**        | JDBC for database connectivity, Swing for GUI |

## Installation

To get started with the Car Membership App, follow these installation steps:

### 1. Clone the repository:
```bash
git clone https://github.com/yourusername/car-membership-app.git
cd car-membership-app


![car](https://github.com/user-attachments/assets/3746e1ed-d62c-4e98-95f5-e58c7d0589b1)

### 2. Set up MySQL Database:
1. Install MySQL on your local machine or use a remote MySQL server.
2. Create a new database named car_membership.
Create a table for storing member information. You can use the following SQL script:

sql
CREATE TABLE members (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    car_model VARCHAR(50),
    license_plate VARCHAR(20),
    membership_type VARCHAR(20),
    contact VARCHAR(50),
    account_number VARCHAR(50)
);


