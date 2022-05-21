## Doc
https://docs.ansible.com/

###
https://docs.ansible.com/ansible/2.5/modules/service_module.html

https://docs.ansible.com/ansible/latest/collections/ansible/builtin/apt_module.html

### Ansible Variables
https://docs.ansible.com/ansible/latest/user_guide/playbooks_variables.html

```
ansible-playbook -i hosts create_user.yml

ansible-playbook -i hosts create_user.yml -e "user=tom"
```

#### tags
```
ansible-playbook -i hosts install_apache_httpd.yml --tags "start_apache"

ansible-playbook -i hosts install_apache_httpd.yml --tags "install_apache"
```

### Ansible Vault
https://docs.ansible.com/ansible/latest/cli/ansible-vault.html

https://docs.ansible.com/ansible/latest/collections/ansible/builtin/git_module.html
```
ansible-vault create vault-pass.yml

ansible-vault view vault-pass.yml
```
### Ansible Roles
https://docs.ansible.com/ansible/latest/user_guide/playbooks_reuse_roles.html
```
ansible-galaxy init setup-apache
```
