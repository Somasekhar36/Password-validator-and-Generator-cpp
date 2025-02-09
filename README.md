# Password Validator and Generator

## Overview
This project provides a robust **Password Validator and Generator** application written in C++. It includes features to assess password strength, ensure password compliance, and generate secure, customized passwords.

## Features
- **Password Validation:**
  - Ensures a minimum password length of 8 characters.
  - Verifies the presence of at least one uppercase letter, one lowercase letter, one number, and one special character.
  - Classifies passwords as `Weak`, `Better`, or `Strong`.

- **Password Generation:**
  - Generates secure passwords based on user input such as name and date of birth.
  - Includes random characters, numbers, and special characters.
  - Customizable password length with a minimum of 8 characters.

- **Interactive User Experience:**
  - Users can either input their own password or let the system generate one.
  - Provides feedback on password strength.

## Usage

### 1. Compile and Run
To compile the code, use the following command in your terminal:
```bash
 g++ -o PasswordApp PasswordValidatorGenerator.cpp
 ./PasswordApp
```

### 2. Input Information
Upon running the program, you'll be prompted to enter your:
- Phone number
- Email
- First and last name
- Date of birth (in `dd mm yyyy` format)
- Department and experience information

### 3. Choose Operation
You will be presented with the following choices:
- **Enter Your Own Password:**
  - Input and confirm your custom password.
- **Generate a Password:**
  - Provide the desired length (minimum 8 characters).
  - Receive a randomly generated password.

### 4. Password Validation
The system will automatically classify the strength of your password based on its complexity.

### Example Output
```
Enter your Phone Number: 1234567890
Enter your email-id: example@email.com
Enter your First Name: Peter
Enter your Last Name: Parker
Do you have any research Publications(Y|N): Y
How many years of experience do you have? 5
Enter your Department: IT
Enter your Date Of Birth (dd mm yyyy): 10 08 2001

Enter your Password(e):
    or
Shall I Suggest a Password(g): g

Enter the desired password length (minimum 8): 12
Generated password: @Pe10r5!*2re
Password is strong!
Do you like the password? (y for YES and n for NO): y
```

## Code Structure
- **PasswordManager:** Base class for password validation.
- **PasswordGenerator:** Derived class to generate secure passwords.
- **Main Function:** Handles user input and interaction logic.

## Requirements
- C++ compiler (G++ recommended)
