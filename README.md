# Deploy Docker Applications from DockerHub with Ansible

## From Public repository of Dockerhub
```bash
$ ansible-vault create vault.yml
(enter new vault password)
$ ansible-playbook docker-ansible-public.yml --ask-vault-pass --ask-become-pass

#To edit your username or password
$ ansible-vault edit vault.yml

$ ansible-playbook docker-ansible-public.yml --ask-vault-pass --ask-become-pass
BECOME password: 
Vault password: 
```

Then access from browser

[http://localhost:1112]

## docker-ansible.yml is for private repository of DockerHub and keep your sensitive data such as dockerhub username and password in Ansible Vault
