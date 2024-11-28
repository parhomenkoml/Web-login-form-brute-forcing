# Web login form brute forcing

This project focuses on developing and executing a brute force attack on a web-based login form. The project is divided into two key components:

- Building a Simple Web Application: A basic web application was created using Flask, with an HTML login page for users to enter their credentials.
- Automating the Brute Force Attack: A Python script was developed to automate login attempts using a dictionary of common passwords, while also monitoring the server responses to identify valid credentials.

Web Application Development

To simulate the target for the brute force attack, a simple Flask-based web application was built. Flask, a lightweight web framework, was used to handle routes and process form submissions. The login page, designed with HTML, provided fields for users to input a username and password.

When a user enters incorrect login credentials, an error message is displayed. On the other hand, if the correct credentials are entered, a success message is shown. These two distinct responses — one for failure and one for success — allow the brute force script to identify whether the login attempt was successful or not.
![Screenshot_2024-11-28_10-54-46](https://github.com/user-attachments/assets/e4d7dbd3-ae61-4cfb-8e9c-ed55ed38e47c)


![2024-11-28 09_36_29-Greenshot](https://github.com/user-attachments/assets/751be1fd-4fb0-455f-b53b-551a93ac2a9e)

Automating the Brute Force Attack

To automate the brute force attack, a Python script was written. The script attempts to find the correct password for a given username by testing multiple passwords from a list (top 100 common passwords).

The script works by iterating through each password and submitting login attempts to the Flask application. If the response indicates a successful login, the script halts and outputs the valid username and password combination.
![Screenshot_2024-11-28_07-45-57](https://github.com/user-attachments/assets/09a2e154-6feb-4bee-8751-f7afa051d1ea)

Upon finding the correct combination, the script outputs a success message, showing the valid username and password.


![Screenshot_2024-11-28_10-35-05](https://github.com/user-attachments/assets/5801b429-238a-46a3-b363-889c650a85e2)

Conclusion

In conclusion, this project demonstrates the vulnerability of web applications to brute force attacks, especially when weak or commonly used passwords are in play. By simulating this attack using a simple Flask application and an automated Python script, we can see how easily an attacker could gain access to an account if proper security measures, such as stronger passwords and rate-limiting, are not implemented. This project highlights the importance of using complex, unique passwords and employing additional layers of security like account lockouts or CAPTCHA systems to mitigate the risks associated with brute force attacks.
