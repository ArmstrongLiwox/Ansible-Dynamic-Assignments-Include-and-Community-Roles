# Ansible Dynamic Assignments (Include) and Community Roles

In the previous projects we performed configurations using playbooks, roles and imports. 

Now we will continue configuring the UAT servers using new Ansible concepts and modules.

In this project we will introduce dynamic assignments by using ***include*** module.

## What is the difference between static and dynamic assignments?

> - Static assignments use ***import*** Ansible module while the module that enables dynamic assignments is ***include***.

# import = Static

# include = Dynamic

> When the ***import*** module is used, all statements are pre-processed at the time playbooks are parsed. 

Meaning, when you execute site.yml playbook, Ansible will process all the playbooks referenced during the time it is parsing the statements. 

This also means that, during actual execution, if any statement changes, such statements will not be considered. Hence, it is static.

> On the other hand, when ***include*** module is used, all statements are processed only during execution of the playbook. Meaning, after the statements are parsed, any changes to the statements encountered during execution will be used.

> ***Take note that in most cases it is recommended to use static assignments for playbooks***, 
because it is more reliable. 

With dynamic ones, it is hard to debug playbook problems due to its dynamic nature. 

However, you can use dynamic assignments for environment specific variables as we will be introducing in this project.


---
> Ansible is an actively developing software project, so the Ansible Documentation will be handy for the latest updates on modules and their usage. https://docs.ansible.com/

---

# Instructions On How To Submit Your Work For Review And Feedback

1. In your https://github.com/ArmstrongLiwox/ansible-config-mgt.git GitHub repository start a new branch and call it ***dynamic-assignments***.

2. Create a new folder, name it ***dynamic-assignments***. 

3. Then inside this folder, create a new file and name it ***env-vars.yml***. 
We will instruct ***site.yml*** to include this playbook later. For now, let us keep building up the structure.

Your GitHub shall have following structure by now.

Note: Depending on what method you used in the previous project you may have or not have roles folder in your GitHub repository - if you used ansible-galaxy, then roles directory was only created on your Jenkins-Ansible server locally. It is recommended to have all the codes managed and tracked in GitHub, so you might want to recreate this structure manually in this case - it is up to you.

















