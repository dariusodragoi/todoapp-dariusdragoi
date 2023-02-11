# Deployment of Todo App using Ansible

This repository contains the necessary files to deploy a todo app using Ansible. 

## Prerequisites

- Ansible installed on my local machine
- Access to an Ubuntu virtual machine in Azure
- An ssh key pair for accessing the virtual machine
- A copy of the todo app code on my local machine

## Contents

The repository contains two files:

- `deploy_todo_app.yml`: This is an Ansible playbook that automates the deployment of the todo app. It installs the necessary packages, adds the Docker repository, copies the todo app code to the virtual machine, and starts the app using Docker Compose.

- `inventory.ini`: This file contains the inventory of the virtual machine, including its IP address and the ssh credentials for accessing it.

## Deployment

- I run the following command to deploy todo app: ansible-playbook deploy_todo_app.yml -i inventory.ini
- You can access this link to see the application in the virtual machine: http://40.114.142.55:3000/
