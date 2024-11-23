                                                   _ **Expense-Management-Systems**_
This is an expense management system which consists of features as follows:
firstly it creates a login using the password and at the same time creates a file of the same name as the login.
You can then sign up and you can add,delete,view or exit the system.
Features
User Management
Create New Account: Allows users to register by providing a unique username and password.
Login: Authenticates users by matching their username and password with stored records.
Expense Management
Add Expense: Users can add new expenses with details such as category, item name, amount, date, and description.
View All Expenses: Displays a list of all expenses in a formatted table.
Delete Expense: Users can remove an expense by specifying the item number.
Save to File: Updates expense records in a file after changes are made.
 Data Storage
User Account Data:
Stored in a file with the format: username,password,filename.csv.
Each user has a dedicated .csv file for storing expenses.
Expense Data:
Stored in a CSV file, with each line representing an expense (category,itemName,amount,date,description).
 Key Functionalities
File Handling
File Opening:
Uses fopen for reading (r), writing (w), or appending (a) files.
Includes error handling to ensure files are opened successfully.
File Reading/Writing:
Reads lines using fgets.
Writes formatted data using fprintf.
Ensures data integrity using fflush.
Dynamic Memory Management
Uses malloc and realloc to dynamically allocate memory for the expenses array as new entries are added.
Ensures memory safety with proper error handling for allocation failures.
 Error Handling
Handles potential errors such as:
File opening failures (perror).
Invalid input for numeric fields.
Memory allocation errors (realloc failures).
 Modular Functions
Modular design for easier understanding and maintenance:
Account Management: createNewAccount, login.
Expense Operations: addExpense, deleteExpense, viewAllExpenses, saveExpensesToFile.
Utility Functions: initializeFile, increaseMemoryForExpenses, extractExpensesFromFile.
 User Interaction
Uses fgets and scanf for input, ensuring users can input data interactively.
Displays clear, formatted output (e.g., tables for expenses).
Provides meaningful error messages and feedback to guide the user.
8. Potential Improvements
Password encryption for enhanced security.
More robust input validation (e.g., checking valid dates).
Improved file handling to avoid potential data corruption (e.g., handling concurrent access).
