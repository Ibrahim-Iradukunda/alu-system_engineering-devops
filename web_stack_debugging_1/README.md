Web Stack Debugging - Task 0: Nginx Likes Port 80
Overview
In this task, you will debug an Ubuntu container running Nginx to ensure that it listens on port 80. After identifying the issues preventing Nginx from listening on port 80, you will write a Bash script to automate the fix. The final goal is for Nginx to serve its default page when accessed on port 80.

Requirements
All files will be interpreted on Ubuntu 20.04 LTS.
Your files should end with a new line.
A README.md file is mandatory and should be placed at the root of the project folder.
All Bash script files must be executable.
Your Bash scripts must pass Shellcheck without any errors.
Your Bash scripts must run without errors.
The first line of all your Bash scripts should be exactly: #!/usr/bin/env bash.
The second line of your Bash scripts should contain a comment explaining what the script does.
You are not allowed to use wget in your solution.
Task Details
Task 0: Nginx Likes Port 80
Objective:

Debug the Nginx installation inside the Ubuntu container to ensure that it is listening on port 80.
Once the issue is identified, write a Bash script to fix it, ensuring Nginx is properly configured and listening on all active IPv4 IP addresses of the server on port 80.
Steps:

The issue is that Nginx is not properly listening on port 80. Your task is to debug and fix this.
The solution should ensure Nginx is running and accessible via port 80 on the container’s active IP addresses.
After the fix, accessing port 80 should return the default "Welcome to nginx!" page when you use a browser or make a request to the server.
Expected Output:

Before fixing the issue, attempting to access port 80 should result in a failure to connect.
After fixing the issue, accessing port 80 should return the default Nginx welcome page.
Deliverables
Bash Script:
Your solution should be placed in the 0-nginx_likes_port_80 file in the GitHub repository.
The script must be executable and should contain only the necessary commands to fix the issue.
Testing:
After running the Bash script, verify that Nginx is correctly listening on port 80.
Conclusion
This project teaches you how to debug and fix an issue with Nginx inside a Docker container, focusing on getting the web server to listen on the correct port. By completing this task, you will enhance your debugging skills and learn how to ensure services like Nginx are properly configured in containerized environments.
