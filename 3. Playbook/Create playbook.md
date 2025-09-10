# Ansible concept

### 1. Playbook
- A playbook is a YAML file that defines the series of actions to be executed on the managed nodes. It contains one or more plays that map the groups of hosts to a role.
- Playbooks are automation blueprints, in YAML format, that Ansible uses to deploy and configure the managed nodes

### Play
- A play is a single, complete execution unit within a playbook.
- It specifies which host to target and what tasks to execute on those hosts.
- Plays are used to group the related tasks and execute them in a specific order
- An ordered list of tasks that maps to managed nodes in an inventory
Example:
```yml
-name: Install and configure nginx
 hosts: webserver
 tasks:
   -name: Install nginx
    apt:
      name: nginx
      state: present
```

### Task
- A reference to a single module that defines the operation that Ansible performs.

### Module
- The unit of code that Ansible runs on managed nodes.
