## System Design: Flask Form Submission Web App

### Overview
The Flask Form Submission Web App is a simple web application built using the Flask framework. It allows users to submit personal details through a form, which are then stored in a SQLite database. Additionally, an email notification is sent to the user's provided email address containing their submitted information.

### Components

1. **Frontend Interface:**
   - User Interface: HTML templates located in the "templates" folder are used to render the user interface. The main page includes a form for users to input their details.
   - Form Submission: Upon submitting the form, user input is sent to the Flask backend for processing.

2. **Flask Backend:**
   - Application Routes: The Flask app defines routes for handling various actions, such as rendering the form page and processing form submissions.
   - Data Handling: Flask-SQLAlchemy manages the SQLite database. Form data is stored in a "Form" table with fields for first name, last name, email, date, and occupation.
   - Email Sending: Flask-Mail is used to send email notifications. When a form is submitted, an email containing the user's details is sent to the provided email address.

3. **Database Management:**
   - SQLite Database: The application uses a SQLite database ("data.db") to store form submissions. The "Form" table structure includes fields for each input field in the form.

4. **Email Sending:**
   - Email Configuration: The application is configured to send emails using Gmail's SMTP server with SSL encryption.
   - Flask-Mail Integration: The Flask-Mail extension is used to create and send email messages. Email content includes the submitted form data.

5. **Instance Configuration:**
   - Configurations: The "instance" folder contains instance-specific configurations for the application, including the secret key, database URI, and email settings.

### Workflow

1. User accesses the web application through a browser.
2. The homepage displays a form where the user can input their details.
3. Upon submitting the form, the data is sent to the Flask backend for processing.
4. The Flask backend stores the form data in the SQLite database.
5. An email notification is sent to the user's provided email address containing their submitted information.
6. The user receives the email and is informed that their form was submitted successfully.
7. The user interface can be further improved with styling and validation.

### Technologies Used

- Flask: Python web framework used for routing and backend logic.
- Flask-SQLAlchemy: Extension for database management and ORM.
- Flask-Mail: Extension for sending email notifications.
- SQLite: Local database for storing form submissions.
- HTML/CSS: Frontend templates and styling for user interface.

This system design provides an overview of the Flask Form Submission Web App's architecture, components, workflow, and technologies. It highlights the key elements that make the application functional and interactive.