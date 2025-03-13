#User Registration Form - Java Swing with MySQL Integration



This is a User Registration System built with Java Swing for the frontend and MySQL for backend database management. The application allows users to enter their personal details and register an account, which gets stored securely in the MySQL database.

<div align="center"> <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white" /> <img src="https://img.shields.io/badge/Swing-%23007396.svg?style=for-the-badge&logo=java&logoColor=white" /> <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" /> </div>


**📌 Features**


✅ Beautiful Graphical User Interface (GUI) built with Java Swing

✅ Collects user details: First Name, Last Name, Username, Email, Mobile Number, and Password

✅ Validates mobile number length (should be 10 digits)

✅ Stores user data into MySQL Database

✅ Provides feedback messages for success or validation failures



**💻 Technologies Used**


| Frontend    | Backend    | Database |
|-------------|------------|----------|
| Java Swing  | Java JDBC  | MySQL    |


**📸 Screenshots**

Registration Form (Java Swing UI)

![Screenshot 2025-03-13 122609](https://github.com/user-attachments/assets/9288b0a3-ecd2-40cf-912b-aa9f58383548)

**⚙️ How It Works**


User Input

Users enter personal details in the registration form (First Name, Last Name, Email, Username, Password, and Mobile Number).

Validation

Mobile numbers are validated (must be exactly 10 digits).

Database Connection

The data is stored into the MySQL database table named account.

Success/Error Message

The user is notified of the registration outcome via JOptionPane.


**🛠️ Prerequisites**


✔️ Java JDK (version 8 or later)

✔️ MySQL Server (running locally or remote)

✔️ MySQL JDBC Connector (version 8.0 or compatible)

✔️ Any IDE (Eclipse, IntelliJ, NetBeans) or text editor

✔️ Basic knowledge of SQL and Java


**⚡ Getting Started**

1.  Clone the repository:
   ```bash
   gh repo clone Ananna-15/-SwingUserReg-
```

2. Create MySQL Database and Table:
```bash

CREATE DATABASE swing_demo;

USE swing_demo;

CREATE TABLE account (
    firstname VARCHAR(50),
    lastname VARCHAR(50),
    username VARCHAR(50) PRIMARY KEY,
    password VARCHAR(50),
    email VARCHAR(100),
    mobile VARCHAR(15)
);
```
3. Add MySQL JDBC Driver
Download the mysql-connector-java from MySQL Downloads
Add it to your project's build path in your IDE.

4. Update Database Credentials
In UserRegistration.java:
```
Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/swing_demo", "root", "your_mysql_password");
```

5. Run the Project
Compile and run UserRegistration.java in your IDE.
Fill in the form and click Register.


**🚀 Future Improvements**


✅ Password hashing for better security

✅ Input validation improvements (email format, password strength)

✅ Login authentication system

✅ CRUD functionality (Update users)




**🤝 Contributing**

Contributions are welcome! Feel free to fork this repository and submit a pull request.
For major changes, please open an issue first to discuss what you'd like to change.


🙋‍♀️ Author
👤 Ananna Das
💼 Java Developer | Frontend Enthusiast
📍 Dankuni, Hooghly
