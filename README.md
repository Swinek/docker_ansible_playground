# Ansible Local Docker Automation

A demonstration project automating the process of installing the Docker engine and deploying containerized applications on a local machine using **Ansible**. 

## Project Overview
The main goal of this project is to replace manual environment configuration with an automated IaC approach. This Ansible Playbook seamlessly prepares the operating system, manages dependencies, and spins up an isolated web application (Nginx) inside a Docker container.

## Tech Stack
* **Ansible** - Configuration management and automation.
* **Docker** - Application containerization.
* **YAML** - Playbook definition format.
* **Kali Linux** - Target operating system.

## Project Structure
* `docker_setup.yml` - The core playbook containing the list of tasks to execute.
* `hosts.ini` - The inventory file defining the target (configured for `localhost`).
* `README.md` - Project documentation.

##  How to Run

### 1. Prerequisites
* Ansible installed on your local machine (`sudo apt install ansible`).
* A Debian-based operating system.

### 2. Execution
Navigate to the project directory and run the following command:
```bash
ansible-playbook -i hosts.ini docker_setup.yml -K