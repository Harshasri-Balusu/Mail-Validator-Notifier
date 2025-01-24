# Mail Validator & Notifier
A Python-based project that validates user details and sends personalized email notifications to users with valid data. This project automates the process of data validation and email delivery, making it an efficient tool for managing user information.

# Features
## Data Validation: Checks the accuracy of user inputs (Name, Gender, DOB, Mobile, and Email) using regular expressions.
## Error Handling: Identifies and skips invalid data entries while notifying about errors.
## Email Automation: Sends customized emails to users with valid information using the SMTP protocol.
## File Handling: Processes user data from a text file.

# Tech Stack
Python: Core language for implementation.
SMTP: For sending email notifications.
Regex: For validating data fields.
File I/O: To read and process user data.

# How It Works
Reads user data from details.txt (a comma-separated file with user details).
Validates each user's information against predefined patterns:
First Name: Only alphabets and spaces.
Last Name: Uppercase alphabets only.
Gender: Either MALE or FEMALE.
Date of Birth: Format DD-MM-YYYY.
Mobile Number: 10-digit numeric values.
Email: Valid Gmail address.
Sends personalized emails to valid users and skips invalid entries with an error message.
# Setup and Usage
## Clone this repository:
bash
Copy
Edit
# git clone https://github.com/yourusername/mail-validator-notifier.git  
## cd mail-validator-notifier  
## Install the required libraries (if not already installed):
bash
Copy
Edit
## pip install smtplib email  
# Edit the script with your Gmail credentials:
python
Copy
Edit
# server.login("your-email@gmail.com", "your-app-password")  
Note: Use an app password for secure authentication.

# Prepare your details.txt file in this format:
graphql
Copy
Edit
FirstName,LastName,Mobile,DateOfBirth,Gender,Email  
John,Doe,9876543210,01-01-2000,MALE,johndoe@gmail.com  
Jane,DOE,8765432109,02-02-1995,FEMALE,janedoe@gmail.com  
Run the script:
bash
Copy
Edit
python mail_validator_notifier.py  
Output
Valid users will receive a personalized email with their details.
Invalid entries will display an error message in the console.

# Future Enhancements
Add support for additional email providers.
Integrate a graphical user interface (GUI) for easier interaction.
Implement logging for detailed error tracking.
