## Ansible Playbooks

- [Document](https://docs.ansible.com/projects/ansible/latest/index.html#)

#### check connection to server using inventory

- [inventory example](https://docs.ansible.com/projects/ansible/latest/getting_started/get_started_inventory.html#use-metagroups)

```
ansible myhosts -m ping -i ansible/inventory.ini
ansible myhosts -m ping -i ansible/inventory.yaml
```

#### run playbook

```
ansible-playbook -i ansible/inventory.yaml ansible/playbook-example.yaml
```
