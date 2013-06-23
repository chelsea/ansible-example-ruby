This is an example set of ansible playbooks using roles which should leave you with a server set up with ruby and postgres.

You must have ansible installed, check out ansible/ansible for details there.

Once ansible is installed, change the [webserver] domain in the hosts file to your domain/IP, then just run:

    ansible-playbook playbook.yml -i hosts
    
If your ssh key is not authorized for the target machine, you can specify a pem file like so:

    ansible-playbook playbook.yml -i hosts --private-key ~/.ssh/sydney.pem
