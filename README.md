# ***Ansible playbook with 2 roles for docker container with PostgreSQL***

My **ansible --version** is: 

> $ ansible --version
*ansible [core 2.12.2]
python version = 3.8.10 (default, Nov 26 2021, 20:14:08) [GCC 9.3.0]
jinja version = 2.10.1
*libyaml* = True*

Fist you need to create 2 roles with command: 
> $ ansible-galaxy init add_docker

> $ ansible-galaxy init create_containers

When you have created a roles ansible automatically creates some directories:
- files
- handlers
- meta
- README.md
- tasks 
- templates 
- tests
- vars

In my example only *vars* and *tasks* are used. You can copy *vars* and *tasks* from my example to your roles directories but first you have to remove the existing ones.

When roles all done you should create *side.yml* and write your roles in this.

After all use the following command to run your playbook: 
> $ ansible-playbook -i /home/ansible/hosts side.yml

Ansible [documentation](https://docs.ansible.com/ansible/latest/index.html) can help you. 

