# Prereqs

- Vagrant
- Ansible

**Clone project**

```bash

git clone https://github.com/jpcasas/ibm-mq-ansible-example.git
cd ibm-mq-ansible-example

```

**Create Machine**

```bash

vagrant up 

```

**Install Ansible MQ Role**

```bash

ansible-galaxy install jpcasas.ibm_mq_ansible_role 


```

**Check vagrant SSH information**

```bash

vagrant ssh-config

```

Copy the information HostName, user, port, IdentityFile and replace it in the inventory.ini file

**Check the connection**

```bash

ansible all -m ping -v

```

**Install Role**

```bash

ansible-playbook playbook-mq.yml

```
**Run Playbook**

```bash

ansible-playbook playbook-mq.yml

```

