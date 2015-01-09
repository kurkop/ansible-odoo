ansible-odoo
============

Playbooks to install and run Odoo, Nginx, Postgres and coming soon uwsgi.

####Clone:
    git clone https://github.com/kurkop/ansible-odoo.git

####Vagrant:
    vagrant up

####Get ssh_key:
    cd && cat .ssh/id_dsa.pub
    
####Access to vagrant, update and create ssh keys:
    vagrant ssh
    apt-get update
    ssh-keygen

####Copy content from id_dsa.pub (Home) to .ssh/authorized_keys (Vagrant)

####Run Ansible Playbooks:
    ansible-playbook -c paramiko -i hosts setup.yml

