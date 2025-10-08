
# Flask on Cloud VM (Assignment 2)

## Student Info
- Name:  Ezzah Asad
- Cloud Provider:  Google Cloud Platform (GCP)

## Video recording: 
- Zoom/Loom: Loom

## Steps
### 1. VM Creation
Selected the **e2-micro machine type (2 vCPU, 1 GB memory)** and the **Ubuntu 25.04 Minimal** OS image. 

![VM_Creation_1](screenshots/creatingvmflask.png)
![VM_Creation_2](screenshots/creatingvmflask_2.png)


### 2. Networking (Port 5003 Open)
 Displays the **networking configuration** for the VM. Enabled **Allow HTTP traffic** and **Allow HTTPS traffic** to permit web requests to the Flask app.  **network interface section**, the primary internal IP and the external IP: **ephemeral** was set at default. 
![Networking_screenshot](screenshots/creatingvmflask3.png)

### 3. OS Update + Python Install
OS and development tools setup process:
Updated and upgraded all Ubuntu packages.
Installed Git, Python 3.13, pip, and venv — in that order to prevent dependency errors and ensured the environment was fully configured for Flask deployment.
![OS_Update](screenshots/sudo_apt_upgrade.png)
![Python_Install](screenshots/installrequiretools.png)

### 4. Flask App Running
Flask app running on port 5003 inside the SSH terminal.
![screenshot of terminal + browser](screenshots/updates_installation.png)
![flask_running](screenshots/flask_running.png)

### 5. Public IP Access
Confirming that the Flask app is accessible through the VM’s public IP address in a web browser.
URL: http://34.44.114.108:5003 
![VM_running](screenshots/vmrunning.png)

### 6. (Bonus) Domain Name
Domain: http://mydomain.tech:5003  
[screenshot]

### Summary
In this project, I successfully deployed a Flask web application on a Google Cloud Virtual Machine. The process included creating a VM instance, configuring firewall rules to open port 5003, updating the operating system, and installing Python, pip, Git, and venv in the correct order. 
I initially encountered several errors when running pip and Flask due to missing dependencies and incorrect installation order. To fix this, I recreated my machine multiple times and carefully reorganized my SSH commands. I started with system updates and then installing the required packages one by one. Once the environment was properly set up, the Flask application launched successfully and was accessible via my public IP address.
