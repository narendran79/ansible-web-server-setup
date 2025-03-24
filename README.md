# ansible-web-server-setup

# Ansible Nginx Setup

This project demonstrates how to use **Ansible** to automate the setup of **Nginx** on EC2 instances.

## Project Structure

- **inventory**: Contains the inventory file (`inventory.ini`) specifying EC2 instances to be managed by Ansible.
- **playbooks**: Contains the Ansible playbook (`web_server_setup.yml`) that installs and configures Nginx.
- **web_service**: Basic (`index.html`)html and (`styles.css`)css page.

## How to Use

1. Clone the repository to your machine.
2. Edit the **`inventory.ini`** file with your EC2 instance IP addresses and SSH key.
3. Run the playbook: ansible-playbook -i inventory/inventory.ini playbooks/web_server_setup.yml
   
   
## Playbook Overview

1. Install Nginx: Installs the Nginx web server.
2. Start Nginx: Ensures that Nginx is started and enabled to start on boot.
3. Firewall Configuration: Configures UFW (Uncomplicated Firewall) to allow HTTP traffic on port 80.
4. Web Page Setup: Deploys a simple index.html and styles.css file to the /var/www/html/ directory.

## Result

![image](https://github.com/user-attachments/assets/659ac3ba-607d-44f8-aa32-6d18fb929bb5)

![image](https://github.com/user-attachments/assets/705dda8d-0eeb-4b48-aa75-486366ec5865)




