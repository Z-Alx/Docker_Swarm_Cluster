# Docker_Swarm_Cluster
Ansible playbook deploy cluster docker swarm

Vagrantfile - разворачивает серверную инфраструктуру
```
vagrant up
```
**deploy.yml** - плейбук кластера

**hosts.ini** - список хостов если раскатывать на виртуалки созданные вагрантом, то менять не надо, если на свои то изменить адреса
```
ansible-playbook --diff -i inventory.ini -u maintenance deploy.yml
```