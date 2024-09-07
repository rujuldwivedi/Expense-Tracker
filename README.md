# Expense Tracker

## Overview

The **Expense Tracker** is a full-featured web application designed to help users manage their personal finances by tracking their daily, weekly, and monthly expenses. Built using Java, Spring Boot, and Java Servlets, this app allows users to add, edit, and delete expenses, categorize them, and view insightful summaries to help better understand spending patterns.

---

## Features

- **User Authentication**: Secure sign-up, login, and logout functionality.
- **Expense Management**: Add, edit, and delete expenses with relevant details like amount, category, and date.
- **Categorization**: Organize expenses under various categories like food, entertainment, transport, etc.
- **Monthly Summaries**: View total monthly expenses and summaries of individual categories.
- **Dashboard**: A user-friendly dashboard displaying graphical representations of spending trends.
- **Responsive UI**: Mobile-friendly interface using HTML, CSS, and Bootstrap for an optimal user experience.

---

## Tech Stack

- **Backend**: Java, Spring Boot, Java Servlets, Hibernate (ORM for database interaction)
- **Frontend**: HTML, CSS, JavaScript, Bootstrap
- **Database**: MySQL (or any relational database of choice)
- **Security**: Spring Security for user authentication
- **Deployment**: Tomcat server, can be deployed to cloud services like AWS or Heroku

---

## Installation and Setup

### Prerequisites
- Java Development Kit (JDK) 8 or higher
- MySQL or any other database
- Apache Maven
- Apache Tomcat server

### Steps to Run Locally

1. **Clone the repository**:
   ```
   git clone https://github.com/rujuldwivedi/expense-tracker.git
   cd expense-tracker
   ```

2. **Configure the Database**:

   *Create a new database in MySQL*:
```
CREATE DATABASE expense_tracker;
```
   *Update the application.properties file in the src/main/resources directory with your database credentials*:
```
spring.datasource.url=jdbc:mysql://localhost:3306/expense_tracker
spring.datasource.username=root
spring.datasource.password=yourpassword
```
3. **Install Dependencies: Use Maven to install all required dependencies**:
```
mvn clean install
```
4. **Run the Application: Start the application using Spring Boot**:
```
mvn spring-boot:run
```
5. **Access the App: The app will be running on http://localhost:8080. Navigate to the URL in your browser to start using the Expense Tracker.**

## Database Schema
Here is the basic structure of the database tables:

- **Users**: Stores user information.
  - `id`, `username`, `email`, `password`
  
- **Expenses**: Stores user expenses.
  - `id`, `user_id`, `amount`, `category`, `description`, `date`

---

## Usage

- **Sign Up/Login**: Users can create an account and log in to access their personal dashboard.
- **Add Expenses**: Users can add expenses with details like category, amount, and date.
- **Edit/Delete Expenses**: Modify or remove expenses from the list.
- **View Summaries**: The dashboard provides a monthly summary of all expenses, helping users track their spending habits.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or report issues to help improve the project.
