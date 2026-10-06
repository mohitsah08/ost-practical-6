# Open Source Technologies - Practical 6

## Practical Title

Deploy a simple app using Nginx/Apache

## Objective

To deploy and verify web applications using Nginx and Apache HTTP server environments:
1. Node.js web application proxied through Nginx reverse proxy.
2. PHP web application served through Apache HTTP server.

## Part A - Nginx / Node.js

- **Installation Verification**:
  - Nginx: `nginx version: nginx/1.31.6`
  - Node.js: `v26.5.0`
  - npm: `11.17.0`
- **Node.js Application**: Built with Node's built-in `http` module in `nginx-node/server.js`, listening on port 3000.
- **Nginx Reverse Proxy Configuration**: Configured in `nginx-node/nginx.conf` listening on port 8080, forwarding all requests to `http://127.0.0.1:3000`.

## Part B - Apache / PHP

- **Apache HTTP Server**: Running Apache 2.4 (`Server version: Apache/2.4.67 (Unix)`).
- **PHP Project**: Located in `apache-php/index.php`.
- **Apache Deployment**: Hosted and served on `http://localhost:8088/Practical-6/`.

## Active URLs

- **Node.js Server**: [http://localhost:3000](http://localhost:3000)
- **Nginx Reverse Proxy**: [http://localhost:8080](http://localhost:8080)
- **Apache / PHP Deployment**: [http://localhost:8088/Practical-6/](http://localhost:8088/Practical-6/)

## Project Structure

```
Practical-6/
├── README.md
├── .gitignore
├── nginx-node/
│   ├── nginx.conf
│   └── server.js
├── apache-php/
│   └── index.php
└── screenshots/
    ├── 01_nginx_installation_verification.png
    ├── 02_project_folder.png
    ├── 03_server_js.png
    ├── 04_node_server_running.png
    ├── 05_node_browser_output.png
    ├── 06_nginx_configuration.png
    ├── 07_nginx_browser_output.png
    ├── 08_xampp_control_panel.png
    ├── 09_apache_running.png
    ├── 10_php_project_folder.png
    ├── 11_index_php.png
    ├── 12_php_browser_output.png
    ├── 13_php_execution_verified.png
    ├── 14_final_project_structure.png
    ├── 15_final_terminal_verification.png
    └── 16_github_repository.png
```

## Screenshots Included

The `screenshots/` directory contains full visual verification of:
- Software installation verification (Nginx, Node.js, npm)
- Project directory organization
- `server.js` code and Node server startup in terminal
- Browser output of Node server on port 3000
- Nginx reverse proxy configuration (`nginx.conf`) and proxy verification on port 8080
- Apache HTTP server status, active PID, and port listening
- `index.php` in `apache-php` directory
- Apache browser output and execution verification on port 8088
- Complete project directory structure
- Terminal verification of all running services and HTTP response headers
- Final GitHub repository publication
