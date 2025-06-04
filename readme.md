# Practical Work II – OOP – Calculator

## Table of Contents
1. [Introduction](#introduction)  
2. [Description](#description)  
   - [Class Diagram](#class-diagram)  
3. [Problems](#problems)  
4. [Conclusions](#conclusions)

---

## Introduction

This readme file contains the process for Practical work 2, which focuses on building a calculator using the **.NET MAUI** application. The application includes extra featues that are usually not seen in a calculator such as user registration, passwords and a converter for different ways of displaying the number (like Octal, Hexidecimal ect).

---

## Description

The Calculator consists of several interfaces and components that work together. It includes:

- **a Login Page**  
  Allows users to log in using their credentials. Includes a password recovery page.

- **a Register Page**  
  Allows new users to register by entering their name, username and password.

- **a Conversor Page**  
  Provides a number converter with many options, including:
  - Binary to Decimal  
  - Decimal to Binary/Octal/Hexadecimal/Two’s Complement  
  - Octal/Hexadecimal/Two’s Complement to Decimal

- **a User Info Page**  
  Displays the user’s information and  the number of operations performed.

- **Validation Rules**  
  - Inputs must be valid based on the selected conversion type.  
  - If the input is invalid, a warning popup appears and the input is cleared.  
  - the Password must be at least 8 characters long and include:
    - 1 uppercase letter  
    - 1 lowercase letter  
    - 1 number  
    - 1 special character  

- **Data Persistence**  
  User information is stored in a file, either `txt`, `csv`, or `json` and is located in the `/files` directory.

### Class Diagram

> _Insert your class diagram here using an image format (e.g. `![Class Diagram](./files/class_diagram.png)`)_  
> _The diagram should include classes such as `User`, `Validator`, `FileHandler`, `Calculator`, `ConversionStrategy`, and GUI page classes (LoginPage, RegisterPage, etc.)_

---

## Problems

Several challenges were encountered during the development of the application:

- **GUI layout responsiveness:**  
  Ensuring a consistent user experience across different platforms using MAUI was sometimes complex.

- **Password validation logic:**  
  Implementing a robust system that enforced all required password rules required careful testing.

- **User input handling:**  
  Supporting only valid conversion inputs while maintaining good UX (e.g., not frustrating the user with unnecessary errors).

- **File storage format decision:**  
  Choosing between `txt`, `csv`, or `json` for storing user data required weighing readability vs. structure and parsing complexity.

- **Class reuse and integration:**  
  Reintegrating and extending the previously developed classes from the guided practical work within the new UI and feature set.

---

## Conclusions

This project provided practical experience in GUI development, input validation, and secure data handling using .NET MAUI and .NET Core 8.0. Key lessons learned include:

- Importance of separating logic from the UI using well-defined classes
- Benefits of persistent storage and the tradeoffs between different file formats
- How to validate and sanitize user inputs in interactive applications
- Building user-friendly interfaces with real-time error feedback

This exercise reinforced good programming practices such as modular design, clear documentation, and consistent code commenting. The skills and patterns developed here can be directly applied to more advanced .NET applications in the future.