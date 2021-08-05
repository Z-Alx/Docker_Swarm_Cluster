# Docker_Swarm_Cluster
Ansible playbook deploy cluster docker swarm

Vagrantfile - разворачивает серверную инфраструктуру
https://learn.hashicorp.com/vagrant

```
vagrant up
```

# Ansible

https://www.ansible.com/

**deploy.yml** - плейбук кластера

**hosts.ini** - список хостов если раскатывать на виртуалки созданные вагрантом, то менять не надо, если на свои то изменить адреса
```
ansible-playbook --diff -i inventory.ini -u maintenance deploy.yml
```