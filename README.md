# homeserver-iac
Ansible Infrastructure as Code for my homeserver

ansible-vault create secret.yml
ansible-vault edit secret.yml

ansible all -m ping

ansible-playbook run.yml -K --ask-vault-pass
-K asks for sudo password, not needed if enabled passwordless sudo