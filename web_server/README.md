# Web Server Automation Project

## Overview

This project focuses on automating the configuration of an Ubuntu 16.04 web server using Bash scripts. The goal is to set up an Nginx web server, configure redirections, set up a domain, and create a custom 404 page.

## Tasks Breakdown

### 0. Transfer a file to the server

- A script (`0-transfer_file`) that transfers a file to a remote server using `scp`.
- Parameters: file path, server IP, username, SSH key path.

### 1. Install Nginx Web Server

- A script (`1-install_nginx_web_server`) to install Nginx and configure it to return "Holberton School for the win!" on the root page.
- Ensures the service runs on port 80.

### 2. Setup a Domain Name

- A domain name (e.g., `mydomain.tech`) is configured with an A record pointing to the server.

### 3. Redirection

- A script (`3-redirection`) to configure Nginx to redirect `/redirect_me` to `https://www.youtube.com/watch?v=QH2-TGUlwu4`.

### 4. Custom 404 Page

- A script (`4-not_found_page_404`) to configure a custom 404 page displaying "Ceci n'est pas une page".

### 5. Beautiful 404 Page

- A well-designed `5-design_a_beautiful_404_page.html` to replace the default error page.

## Usage

1. Clone the repository.
2. Run each script in order on an Ubuntu 16.04 server.
3. Verify changes using `curl` commands.

## Notes

- Scripts must be executable: `chmod +x filename`
- Use `./script_name` to run each script.
- Ensure DNS records have propagated before testing the domain setup.


