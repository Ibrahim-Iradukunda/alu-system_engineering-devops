# Load Balancer Setup

## Overview
This project configures two web servers behind a load balancer using HAProxy and includes a custom HTTP header to track which server handles each request.

## Setup
1. **Web Servers**: Run `0-custom_http_response_header.sh` to set up Nginx with a custom HTTP header.
2. **Load Balancer**: Run `1-install_load_balancer.sh` to install and configure HAProxy.

## Testing
Use `curl` to check the `X-Served-By` header and verify traffic distribution.

