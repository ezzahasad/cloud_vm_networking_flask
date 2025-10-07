# cloud_vm_networking_flask

### AHI 504 — Assignment 2  
**Deploying a Flask Web App on a Google Cloud VM**

---

### Student Information
- **Name:** Ezzah Asad  
- **Cloud Provider:** Google Cloud Platform  
- **Video Recording:** Loom  


---

## Steps

### Step 1: VM Creation  
This screenshot shows the creation and configuration of the virtual machine on Google Cloud.  
![creating vm flask 2.png)
![creating vm flask.png)

---

### Step 2: Networking (Port 5003 Open)  
This screenshot shows the networking settings with port 5003 open to allow Flask web traffic.  
![creating vm flask 3.png)

---

### Step 3: OS Update + Python Install
Below are the main commands I used to update the system and install the required tools.

```bash
sudo apt update -y  
sudo apt upgrade -y  
sudo apt install git -y  
sudo apt install python3.13 -y  
sudo apt install python3.13-venv python3-pip -y

![sudo apt upgrade.png)
![install require tools (python, git, pip, venv).png)




### Step 4: Flask App Running 
After installing Python, pip, and Git, I cloned the Flask Starter repository and set up a virtual environment. I then installed all required dependencies and ran the Flask application.

![updates_installation.png)
![flask running.png)

```bash
git clone https://github.com/hantswilliams/HHA-504-2025-FlaskStarter.git  
cd HHA-504-2025-FlaskStarter  
python3 -m venv venv  
source venv/bin/activate  
pip install -r requirements.txt  
python3 app.py

5. Public IP Access
URL: http://34.44.114.108:5003
[flask running.png]