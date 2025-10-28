📚 BookPilot Manager

BookPilot Manager is a Library Management System built using Core Java, Advanced Java, and MySQL Database — developed in Apache NetBeans IDE.
It provides librarians and administrators with a clean, efficient, and automated way to manage books, users, and transactions.


---

🚀 Project Overview

BookPilot Manager is designed to simplify the traditional library process by automating key tasks such as book issue/return, student record maintenance, and inventory management.
It provides a secure and efficient way to handle data, eliminating manual errors and paperwork.


---

🧠 Key Features

🔐 User Authentication System — Admin login for secure access.

📘 Book Management — Add, edit, delete, search, and view books.

👨‍🎓 Student/Member Management — Maintain records of members or students.

📥 Issue/Return Module — Track which user borrowed which book and manage due dates.

📊 Transaction History — View all issue/return operations.

📂 Database Integration — Data stored securely using MySQL.

🖥 Interactive GUI — Built with Java Swing & AWT (JFrame-based GUI).

🧾 Reports/Records View — Access details quickly through dynamic search panels.

⚙ Error Handling & Validation — Ensures clean input and stable system behavior.



---

💾 Download Ready-to-Use Version

You can directly download the latest executable from GitHub Releases:

👉 Download BookPilot Manager JAR

Then run:

java -jar LMS.jar




---

🏗 Tech Stack

Category	Technology

Language	Java (Core + Advanced Java)
Database	MySQL
IDE	Apache NetBeans
Libraries Used	rs2xml.jar, rscalendar.jar, rsfoot.jar, mysql-connector-java.jar, others
UI Toolkit	Swing (JFrame Forms)
Build Tool	Ant (default NetBeans build system)



---

🧩 Project Structure

BookPilotManager/
│
├── src/
│   └── com/bookpilotmanager/
│       ├── Login.java
│       ├── Dashboard.java
│       ├── AddBook.java
│       ├── IssueBook.java
│       ├── ReturnBook.java
│       ├── AboutUs.java
│       └── ...
│
├── lib/
│   ├── rscalendar.jar
│   ├── rsfoot.jar
│   └── mysql-connector-java.jar
│
├── nbproject/
├── build.xml
├── manifest.mf
├── README.md
└── .gitignore


---

⚙ Installation & Setup Guide

Follow these steps to run BookPilot Manager on your local system:

1️⃣ Prerequisites

Java JDK (version 8 or above)

Apache NetBeans IDE

MySQL Server & MySQL Workbench


2️⃣ Clone the Repository

git clone https://github.com/yourusername/BookPilotManager.git

3️⃣ Open the Project

Open Apache NetBeans

Go to File → Open Project

Select the BookPilotManager folder.


4️⃣ Setup Database

1. Open MySQL Workbench.


2. Create a new database:

CREATE DATABASE bookpilot;


3. Import the provided SQL file (if included), or manually create tables:

CREATE TABLE books (
    id INT AUTO_INCREMENT PRIMARY KEY,
    title VARCHAR(255),
    author VARCHAR(255),
    publisher VARCHAR(255),
    quantity INT
);

(Add similar tables for students, issue records, etc.)


4. Update your DB configuration in the code (example in DBConnection.java):

String url = "jdbc:mysql://localhost:3306/bookpilot";
String user = "root";
String password = "yourpassword";



5️⃣ Add Required Libraries

Copy all .jar files (like mysql-connector-java.jar, rscalendar.jar, etc.) inside lib/ folder.

In NetBeans, right-click project → Properties → Libraries → Add JAR/Folder → select all from lib/.


6️⃣ Run the Project

Click Run ▶ in NetBeans or press Shift + F6.


---

🧮 Modules Overview

Module	Description

Login	Authenticates admin credentials.
Dashboard	Displays options like Add Book, Issue Book, etc.
Add Book	Allows adding new books to the database.
Issue Book	Handles book issuance to users.
Return Book	Manages book returns and due dates.
About Us	Displays project and developer information.



---

🛡 Security & Validation

Input fields are validated to prevent empty or invalid entries.

Database connection handled using JDBC with proper exception handling.

Restricted admin access for sensitive operations.



---

🧰 Tools & Environment

Tool	Purpose

Apache NetBeans	Project development & GUI Design
MySQL	Database management
Git & GitHub	Version control & hosting
JDK	Java Runtime & Compilation



---

🤝 Contributors

Name	Role

Karan Jha	Developer, Designer, and Project Lead



---

📄 License

This project is open-source and available under the MIT License.


---

💬 Acknowledgements

Special thanks to:

NetBeans IDE 

MySQL for database support

Java community tutorials and documentation for guidance



---

🧭 Future Enhancements

🌐 Migrate project to Spring Boot for web-based access

🔒 Add JWT-based authentication

📱 Build responsive UI using JavaFX or web frontend (React)

☁ Deploy MySQL on cloud (e.g., MongoDB Atlas, Render, etc.)
