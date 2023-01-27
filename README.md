# homeserver-iac
Ansible Infrastructure as Code for my homeserver

ansible-vault create secret.yml
ansible-vault edit secret.yml

ansible all -m ping --ask-vault-pass

ansible-playbook run.yml -K -k --ask-vault-pass
-k asks for SSH password
-K asks for sudo password, not needed if enabled passwordless sudo

ansible-playbook run.yml -l catriel -K --ask-vault-pass -> targets that server

ansible-galaxy install -r requirements.yml