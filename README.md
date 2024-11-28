# Web login form brute forcing

This project revolves around developing and executing a brute force attack on a web-based login form. The project was divided into two main components:

- Building a simple web application using Flask with an HTML login page.
- Developing a Python script to automate brute force login attempts by using a dictionary of common passwords and monitoring server responses.

The web application acted as the target for brute-forcing attempts, simulating a scenario where weak login credentials are used, and the brute force attack helps identify the correct username and password combination.

To simulate a login form for the brute force attack, a simple Flask-based web application was created. Flask was used as the backend framework to manage routes and process form submissions. The login page itself was constructed with HTML, allowing users to input a username and password for submission.
![Screenshot_2024-11-28_07-41-55](https://github.com/user-attachments/assets/0f1c0f07-202d-4059-b06c-477412f70c81)

If a user enters an invalid username or password, an error message will appear. If the credentials are valid, a success message will be displayed. Now, we have two different responses from the app, which can be used to determine whether the inputs are valid or not.

![Screenshot_2024-11-28_07-41-55](https://github.com/user-attachments/assets/5bd96b74-adb3-4a7a-89db-cede6e123b0c)

 

to automate this process we can use python script
The code below is a simple script that attempts to find the correct password for a list of usernames by testing multiple passwords from a file.

![Screenshot_2024-11-28_07-45-57](https://github.com/user-attachments/assets/09a2e154-6feb-4bee-8751-f7afa051d1ea)
