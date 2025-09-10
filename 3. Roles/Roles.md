# Ansible Roles
An Ansible role is a reusable, self-contained unit of automation that is used to organise and manage tasks, variables, files, templates, and handlers in a structured way.

This modular approach promotes reusability, maintainability, and consistency across different playbooks and environments.

# Key component of Ansible Role.

### 1. Tasks:
The main list of actions that the role performs.

### 2. Files:
Static file that needs to be transferred to managed hosts.

### 3. Templates:
Jinja2 templates that can be rendered and transferred to managed hosts

### 4. Vars:
A variable that is used within the role

### 5. Default:
Default variable for the hosts that can be overridden.

### 6. Meta:
Metadata about the roles, including dependencies on other roles.

### 7. Library:
Custom modules are plugins used within the role.

### 8. Module Default:
Default module parameters for the role.

### 9. lookup plugins:
Custom lookup plugins for the roles.

# Directory structure of Ansible Roles:
```
<role_name>/
  ├── defaults/
  │   └── main.yml
  ├── files/
  ├── handlers/
  │   └── main.yml
  ├── meta/
  │   └── main.yml
  ├── tasks/
  │   └── main.yml
  ├── templates/
  ├── vars/
      └── main.yml
```
## Why Use Ansible Roles?

### Modularity
Roles allow you to break down complex playbooks into smaller, reusable components. 
Each role handles a specific part of the configuration or setup.

### Reusability
Once created, roles can be reused across different playbooks and projects. This saves time 
and effort in writing redundant code.

### Maintainability
By organizing related tasks into roles, it becomes easier to manage and maintain the code. 
Changes can be made in one place and applied consistently wherever the role is used.

### Readability
Roles make playbooks cleaner and easier to read by abstracting away the details into logically
named roles.

### Collaboration
Roles facilitate collaboration among team members by allowing them to work on different parts
of the infrastructure independently.

### Consistency
Using roles ensures that the same setup and configuration procedures are applied uniformly across
multiple environments, reducing the risk of configuration drift.
