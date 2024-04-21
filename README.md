## User-Authentication-With-Security-Logs

### **Python Project Overview** 💻

This project is a User Authentication System implemented using Python and Streamlit. It provides a secure platform for managing user accounts, enabling secure login, account creation, password recovery, and activity logging. The system uses SQLite for database management and is designed to provide basic yet crucial security features suitable for educational or small-scale application prototypes.

*****

### **Features**
- **User Registration**: Allows new users to create an account by providing a username, email, and password.
- **Login System**: Supports user authentication to verify identity and grant access to secured areas.
- **Password Recovery**: Includes a mechanism for users to recover and reset their passwords in case they forget them.
- **Security Logging**: Logs all security-related events, including user logins, logouts, and password changes, providing an audit trail for compliance and security monitoring.
Password Reset: Users can change their passwords through a secure interface.

*****

### **Technology Stack**
- **Python**: The core programming language used for backend development.
- **Streamlit**: A Python library for creating and sharing beautiful, custom web apps for machine learning and data science.
- **SQLite**: A C-language library that implements a small, fast, self-contained, high-reliability, full-featured SQL database engine.
- **Hashlib**: For secure hashing of passwords using SHA-256.

*****

## **Installation**
To run this application, you will need Python installed on your system.

### **Cloning the Repository**
First, clone the repository to your local machine:
```
`git clone https://github.com/savakroth/User-Authentication-With-Security-Logs.git`
```

### **Installing Dependencies**
Install the required Python libraries:
```
`pip install -r requirements.txt`
```

### **Setting Up Sender Email**
Inside the `email_request.py`, modify the **sender_email** and **sender_password** variables to set up the verification feature of this app.
- **sender_email** : The email address which will be used to send verification codes
- **sender_password** : The Gmail App Password of the email account

**To get Gmail App Password:**
> Go to google Account -> Enable 2FA -> App Password -> Create new App Password
An App password generated by google should look something like this **"alsl eooq appq sicw"**
Remove the spaces and pass them to the **sender_password** variable

### **Setting Up Table Plus To View Real Time Data**
> Install Table Plus from the official website -> Make a connection towards the directory database file `database.db` which will be created automatically after running `streamlit run main.py`

### **Usage**
To run the application:
```
`streamlit run main.py`
```
This will start the server, and you should be able to access the application by navigating to **http://localhost:8501** in your web browser.







