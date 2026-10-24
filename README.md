# Government-complaint-system_bahhaja_905006101
Government Citizen Complaint Management System

1. Project Overview

The Government Citizen Complaint Management System is a Python-based application developed to help manage complaints submitted by citizens to government offices. It allows users to submit complaints, view all complaints, search for a specific complaint, and update complaint statuses.

The system is developed using Object-Oriented Programming (OOP) concepts in Python.

2. Problem Statement

Citizens may experience difficulties reporting community problems such as poor waste collection, damaged roads, and other public service issues. When complaints are not properly organized, tracking and managing them can become difficult.

This project provides a simple digital system for recording and managing citizen complaints.

3. Project Objectives

The objectives of this project are to:

- Allow citizens' complaints to be recorded.
- Display all submitted complaints.
- Search for complaints using their identification numbers.
- Update the status of complaints.
- Demonstrate the use of Object-Oriented Programming in Python.
- Support more organized complaint management.

4. Technologies Used

- Programming Language: Python
- Development Environment: PyCharm
- Version Control: Git
- Code Hosting Platform: GitHub

5. System Features

Submit a Complaint

Users can enter a complaint ID, citizen name, complaint category, and description.

View All Complaints

The system displays the details of all complaints submitted during the current session.

Search for a Complaint

Users can search for a complaint by entering its complaint ID.

Update Complaint Status

Users can update a complaint's status, for example, from Pending to In Progress or Resolved.

Exit the System

Users can exit the application through the main menu.

6. Object-Oriented Programming Concepts

Classes and Objects

The system uses two classes: "Complaint" and "ComplaintManagementSystem".

The "Complaint" class represents an individual complaint. The "ComplaintManagementSystem" class manages complaint records and the available operations.

Encapsulation

Complaint information is stored in attributes belonging to each complaint object, while methods are used to display information and update its status.

Constructors

The "__init__()" method initializes complaint details and sets the default status to Pending.

Methods

Methods perform specific tasks, including adding complaints, displaying records, searching for complaints, and updating statuses.

Lists

A Python list stores complaint objects during program execution.

7. How to Run the Project

1. Install Python on your computer.
2. Open PyCharm.
3. Open the project folder.
4. Ensure the Python file is named "government_citizen_complaint.py".
5. Open the Python file.
6. Click the Run button.
7. Follow the instructions displayed in the terminal.

8. How to Use the System

After running the program, a menu will appear with five options:

1. Submit a Complaint
2. View All Complaints
3. Search for a Complaint
4. Update Complaint Status
5. Exit

Enter the number corresponding to the operation you want to perform.

9. Limitations

- Complaint records are stored in memory.
- Records disappear when the program closes.
- The current version does not use a database.
- The application does not provide a graphical user interface.
- The program does not include user authentication.

10. Future Improvements

Future versions could include:

- A database for permanent complaint storage.
- User accounts and authentication.
- A graphical user interface.
- Complaint tracking and notifications.
- Reports showing the number and status of complaints.
- Access controls to protect citizens' personal information.

11. Digital Public Good Potential

The project demonstrates how digital technology can help organize public service information and complaint management.

With further development, documentation, privacy protections, accessibility improvements, and an appropriate open-source licence, the system could be adapted for use by different communities or public institutions.

The current project is a basic educational prototype and has not been assessed or certified as a Digital Public Good.

12. Conclusion

The Government Citizen Complaint Management System demonstrates how Python and Object-Oriented Programming can be used to develop a simple application for managing citizen complaints. It provides basic functions for submitting, viewing, searching, and updating complaints while creating a foundation for future improvements.

Author

Developed as a PROG211 Object-Oriented Programming project.
