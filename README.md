
# Doctor Appointment Booking System using PHP

The Home Health Check Management System is designed to provide users with a convenient and accessible platform for remote health monitoring. This web application aims to centralize health data management, allowing users to track vital signs, medication adherence, and communicate with healthcare providers effectively.
## Objectives
The primary objectives of the Home Health Check Management System are:
+ Enhance Efficiency: By automating health data management tasks, the system aims to improve the efficiency of remote health monitoring, enabling users to focus on their well-being rather than administrative tasks.
+ Improve User Experience: The system will provide a user-friendly interface for tracking vital signs, medication schedules, and communicating with healthcare providers, enhancing the overall user experience.
+ Increase Accessibility: By offering remote access to health data and healthcare services, the system aims to increase accessibility to healthcare, particularly for individuals with mobility limitations or living in remote areas.
## Scope of the Project
The scope of this project centres on the development of essential functionalities for remote health monitoring, including vital signs tracking, medication adherence, communication with healthcare providers, health data visualization, and ensuring privacy and security of user data. 

These core features aim to provide users with a comprehensive platform for managing their health remotely and facilitating efficient communication with healthcare professionals. 

While future iterations may expand to include integration with wearable health devices, telemedicine services, and advanced analytics, the initial focus remains on delivering fundamental capabilities to support remote health monitoring effectively.




# SYSTEM REQUIREMENTS
This chapter outlines the system requirements necessary for the development and deployment of the Home Health Check Management System (HHCMS) tailored for remote health monitoring. It details the front-end and back-end tools utilized in the project.
## Front End Tools
For the front-end development of the HHCMS, HTML and CSS were primarily utilized. 
+ HTML (Hypertext Markup Language) is the standard markup language used to create the structure of web pages, while CSS (Cascading Style Sheets) is used to style and format these web pages. These tools provide the foundation for creating a visually appealing and user-friendly interface for the HHCMS.
+ HTML enables the creation of structured content, such as forms for data entry and tables for displaying inventory information, while CSS allows for customization of the layout, typography, and colour scheme to enhance usability and aesthetics.

  
## Back End Tools
The back-end infrastructure of the HHCMS uses PHP and MySQL, facilitated through the XAMPP control panel. 
+ PHP (Hypertext Preprocessor) is a server-side scripting language used for dynamic web development, facilitating data processing and logic implementation behind the scenes.
+ MySQL, an opensource relational database management system, is enlisted for efficient storage and retrieval of data. XAMPP, a comprehensive web server solution bundle, encompasses Apache, MySQL, PHP, and Perl, furnishing an integrated development environment for local web application construction and testing.

By harnessing PHP and MySQL via the XAMPP control panel, the HHCMS adeptly manages inventory data, executes CRUD (Create, Read, Update, Delete) operations, and dynamically generates content in response to user interactions.




# DESIGN
This chapter delves into the design phase of the Home Health Check Management System (HHCMS). It encompasses the depiction of schema and entity-relationship (ER) diagrams, providing a visual representation of the system's database architecture and data model
## Schema Diagram

## ER Diagram of HHCMS

# IMPLEMENTATION
XAMPP is not directly involved in creating a DBMS project as it's a software suite, not a project creation tool. However, it provides the necessary environment to run a DBMS like MySQL and manage databases for your project. PHP is a server-side scripting language that is widely used and open source. It is used to create dynamic webpages. MySQL is an RDBMS software used for storing and organizing data in a structured format using tables and relationships.
## Installation Steps for Execution of the Project
+ Download and Install XAMPP: Head to the official XAMPP website and download the appropriate installer for your operating system https://www.apachefriends.org/. Run the downloaded installer and follow the onscreen instructions.
+ Start XAMPP Services: Open the XAMPP Control Panel, which should be created upon installation. Click the "Start" buttons next to the "Apache" and "MySQL" services. Verify that both services are running green, indicating they are active.
+ Access phpMyAdmin: Open the web browser and navigate to http://localhost/phpmyadmin. This will open the phpMyAdmin interface, a web based tool for managing MySQL databases.
+ Create and Manage Your Database: Once logged in to phpMyAdmin, we can create new databases, manage existing ones, and perform various database operations like creating tables, inserting data, and querying data.

## Project File Structure
The project file structure organizes various components of the Remote Healthcare Management System, including CSS files, directories for admin, doctor, and patient-related pages, along with essential PHP scripts for database connection, account creation, and HTML files for login and signup pages.


Remote_Healthcare_Management_System/<br>
│<br>
├── css/ # Directory for CSS files<br>
│ ├── fonts/ # Directory for font files<br>
│ │ └── inter/ # Directory for Inter font files<br>
│ │ └── cssStyles.css # CSS styles for Inter font<br>
│ ├── admin.css # CSS styles for admin pages<br>
│ ├── animations.css # CSS styles for animations<br>
│ ├── font-inter.css # CSS styles for Inter font<br>
│ ├── index.css # CSS styles for index page<br>
│ ├── login.css # CSS styles for login page<br>
│ ├── main.css # Main CSS styles<br>
│ ├── patient.css # CSS styles for patient pages<br>
│ └── signup.css # CSS styles for signup page<br>
│
<br>├── admin/ # Directory for admin-related pages
<br>│ ├── index.php # Admin dashboard page
<br>│ ├── add_doctor.php # Page for adding new doctors (Admin)
<br>│ ├── edit_doctor.php # Page for editing existing doctors (Admin)
<br>│ ├── delete_doctor.php # Page for deleting doctors (Admin)
<br>│ └── view_patients.php # Page for viewing patient details (Admin)
<br>│
<br>├── doctor/ # Directory for doctor-related pages
<br>│ ├── appointment.php # Page for doctor's appointments
<br>│ ├── delete-appointment.php # Page for deleting appointments (Doctor)
<br>│ ├── delete-session.php # Page for deleting sessions (Doctor)
<br>│ ├── doctors.php # Page for managing doctor's appointments (Doctor)
<br>│ ├── edit-doc.php # Page for editing doctor's information (Doctor)
<br>│ ├── index.php # Doctor's dashboard page
<br>│ ├── patient.php # Page for managing patient details (Doctor)
<br>│ ├── schedule.php # Page for managing doctor's schedule (Doctor)
<br>│ └── settings.php # Page for managing doctor's settings (Doctor)
<br>│
<br>├── patient/ # Directory for patient-related pages
<br>│ ├── appointment.php # Page for patient's appointments
<br>│ ├── booking-complete.php # Page for booking completion (Patient)
<br>│ ├── booking.php # Page for booking appointments (Patient)
<br>│ ├── delete-account.php # Page for deleting patient's account (Patient)
<br>│ ├── delete-appointment.php # Page for deleting appointments (Patient)
<br>│ ├── doctors.php # Page for browsing doctors (Patient)
<br>│ ├── edit-user.php # Page for editing patient's information (Patient)
<br>│ ├── index.php # Patient's dashboard page
<br>│ ├── patient.php # Page for managing patient's appointments (Patient)
<br>│ ├── schedule.php # Page for managing patient's schedule (Patient)
<br>│ └── settings.php # Page for managing patient's settings (Patient)
<br>│
<br>├── connection.php # PHP script for database connection
<br>│
<br>├── create-account.php # PHP script for account creation
<br>│
<br>├── index.html # Main HTML file
<br>│
<br>├── login.php # Login page
<br>│
<br>└── signup.php # Signup page

## Features
### Admin
  
- Admin can add doctors, edit doctors, delete doctors    
- Schedule new doctors sessions, remove sessions   
- View patients details    
- View booking of patients    
    
    
 
 
### Doctors

- View their Appointment
- View their scheduled sessions
- View details of patients
- Delete account    
- Eedit account settings
    

    
### Patiens(Clients)
  
  - Make appointment online
  - Create accounts themslves
  - View their old booking
  - Delete account
  - Edit account settings    



# Login Page
The Login Page is a critical component of the Remote Healthcare Management System, facilitating user authentication and access to their accounts.
+ <b>index.html</b> <br>
The main HTML file serves as the primary entry point for the web application. It defines the structure and layout of the homepage, including navigation elements, headers, and introductory content, providing users with a starting point for accessing other features of the system.

+ <b>connection.php</b> <br>
This PHP script establishes a secure connection to the database for the Remote Healthcare Management System, ensuring seamless data interaction between the web application and the database.

+ <b>For Admin and Doctors: login.php</b> <br>
The login page allows users to authenticate themselves and access their accounts securely. This PHP file processes user login requests, verifies credentials against stored data in the database, and grants access to authenticated users upon successful authentication.

+ <b>For Patients: Account Creation: signup.php , create-account.php</b> <br>
Patients can create accounts independently by accessing the "signup.php" page where they input necessary details. Upon submission, the server-side script "create-account.php" processes the data, validating and creating a new user account in the system's database. Upon successful registration, patients can access various features.

+ <b>account.php</b> <br>
This PHP script is responsible for handling account creation functionality within the system. It provides the necessary backend logic to process user inputs, validate information, and store new account details securely in the database.



