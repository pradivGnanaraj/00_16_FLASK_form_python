
# Form Submission Web App using Flask

This is a simple web application built with Flask that allows users to submit a form with their personal details, which are stored in a SQLite database. Upon submission, an email is sent to the user's provided email address with their form data.

## Getting Started

1. Clone this repository to your local machine.
2. Make sure you have [Python](https://www.python.org/) installed.
3. Install the required packages using the following command:

   ```bash
   pip install -r requirements.txt
   ```

4. Configure the app settings in the `app.py` file:
   - Replace `"YOUR EMAIL"` with your Gmail address in `MAIL_USERNAME`.
   - Replace `"YOUR EMAIL PASSWORD"` with your Gmail password in `MAIL_PASSWORD`.

5. Run the application:

   ```bash
   python app.py
   ```

6. Open your web browser and go to `http://localhost:5001` to access the application.

## Features

- User-friendly form submission interface.
- Form data is stored in a SQLite database.
- Upon submission, a confirmation email is sent to the user's provided email address.
- Use of Flask-Mail for sending emails.
- Utilization of SQLAlchemy for database management.

## Folder Structure

- `instance/`: Contains instance-specific configuration settings (e.g., secret key).
- `templates/`: HTML templates for rendering the web pages.
- `app.py`: The main application script that defines routes and functionality.
- `data.db`: SQLite database file that stores form submissions.

## Dependencies

- Flask
- Flask-SQLAlchemy
- Flask-Mail

## Contributing

Contributions to improve and enhance this project are welcome! Feel free to open issues or submit pull requests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```
