# Konzek Candidate Task-1
This document contains the steps for deploying a simple Flask application on a Linux system, managing it as a Systemd service, and configuring it to start automatically. Flask is a Python-based micro web framework commonly used for creating HTTP servers.

## Installation

Save this code to a file, for example, `app.py`. You can use the following commands to install Flask:

```bash
pip install flask
```
### Loading and Starting the Service Unit
```bash
sudo cp app.service /etc/systemd/system/
```
### Load the service unit:
```bash
sudo systemctl daemon-reload
```
### Start the service:
```bash
sudo systemctl start app-py.service
```
#### You can use the following command to get information about the service status:

```bash
sudo systemctl status app-py.service
```

### Testing the Application

To ensure that your application is working correctly, follow these steps:
Open your browser and go to `http://<localhost>:8080`. You should see the message "KONZEK-CASE-2025."


