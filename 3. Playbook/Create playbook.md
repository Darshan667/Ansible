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

### 3. Modules
- Modules are the building blocks of Ansible tasks.
- They are small programs that perform a specific action on managed nodes, such as installing a package, copying a file, or managing the services.
- Example:
- The apt module is used to install the package
```yaml
- name: Install nginx
  ansible.builtin.apt:
   name: nginx
   state: present
```

### 4. Tasks
- Tasks are individual actions within a play that use the modules to operate on managed nodes. Each task is executed in order and can include conditionals, loops, and handlers
```
tasks:
 - name: Install nginx
   ansible.builtin.apt:
      name: nginx
      state: present
```

### 5. Collections
- Collections are a distribution format for Ansible content.
- They bundle together multiple roles, modules, and other Ansible artefacts.
```yaml
- name: Install nginx
  community.general.module:
  option: value
