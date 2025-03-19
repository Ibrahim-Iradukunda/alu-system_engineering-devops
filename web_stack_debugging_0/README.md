Web Stack Debugging - Task 0: Give Me a Page
Overview
This project focuses on debugging a web server running inside a Docker container. The goal is to ensure that an Apache web server is running correctly inside the container and serves a page with the content "Hello Holberton" when accessed on port 8080.

The task involves manually fixing the web server configuration to get it working and then automating the process with a Bash script.

Requirements
The solution must be implemented in a Docker container.
All solutions should be written in Bash.
The Bash script should be executable.
The script should pass Shellcheck without any errors.
The script must begin with the correct shebang (#!/usr/bin/env bash).
The second line of the script must contain a comment explaining what the script does.
The script files must end with a newline.
The solution should be compatible with Ubuntu 14.04 LTS or a similar environment.
Task Details
Task 0: Give Me a Page
Objective: After running the Docker container, you need to ensure that Apache is installed and configured to serve a page that displays "Hello Holberton" when accessed via port 8080.

Steps:

Install and configure Apache web server inside the Docker container.
Create a simple HTML page that displays the message "Hello Holberton".
Start Apache and ensure it is listening on port 80 inside the container, which maps to port 8080 on the host machine.
Verification:

Once the Docker container is running, verify that the page can be accessed by sending a curl request to port 8080 on the host machine.
The expected response should be the string Hello Holberton.
Deliverables
Your solution should be stored in the 0-give_me_a_page file in your GitHub repository.
The script file must be made executable using chmod +x 0-give_me_a_page.
Ensure that the script ends with a newline character.
The script must be correctly formatted and pass Shellcheck without any errors.
Conclusion
This project teaches you how to debug a web server running inside a Docker container and how to configure Apache to serve static content. You will learn key debugging skills necessary for working with web stacks in Dockerized environments.
