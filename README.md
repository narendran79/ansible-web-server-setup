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
   
   
Playbook Overview
*Install Nginx: Installs the Nginx web server.
*Start Nginx: Ensures that Nginx is started and enabled to start on boot.
*Firewall Configuration: Configures UFW (Uncomplicated Firewall) to allow HTTP traffic on port 80.
*Web Page Setup: Deploys a simple index.html and styles.css file to the /var/www/html/ directory.
