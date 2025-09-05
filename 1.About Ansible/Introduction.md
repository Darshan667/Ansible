# Ansible

### What is Ansible?
Ansible is an open source automation tool that is used for:
1. Configuration Management
2. Application Deployment
3. Task Automation
4. Orchestration

## Configuration Management?
Configuration management is the managing and maintaining of the computer system, servers and software settings.

## Application Deployment?
Ansible can automate the installation or update of the application across different servers.

## Task Automation?
Ansible helps run routine tasks like update, reboot, or service restart.

## Orchestration?
Coordinating the multiple systems and services to work smoothly

## Diagram
<img width="350" height="201" alt="image" src="https://github.com/user-attachments/assets/3a732e12-ab3a-4243-b890-48fd4786168d" />

## How Ansible works?
Ansible works by connecting to the target machines over SSH and then executing the task based on the instructions given in a YAML playbook.

Agentless: You don't need to install anything onto the target machine; it uses SSH to connect and run the tasks

YAML: Task and operation written in a simple YAML file called playbook

Ansible is work by connecting to our nodes/servers and pushin put small programs via ssh called ansible modules to them. 
Ansible then execute these modules. and remove them when finished.

