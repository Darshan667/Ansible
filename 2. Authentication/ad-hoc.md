# Why use an ad-hoc command?
- ad-hoc commands are great for tasks you repeat rarely.
- For example, if you want to power off all machines in your lab for Christmas vacation, you can execute a quick one-liner in Ansible without writing a playbook.
- ```ansible
  ansible [pattern] -m [module] -a "[module options]"
  ```
  
