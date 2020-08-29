Ansible playbook for a fault tolerant PostgreSQL cluster using repmgr.

[MORE ABOUT CLUSTER](https://masya.github.io/postgresql/2020/07/04/postgres-part-05.html)

Tested on Vagrant ubuntu/bionic64, Ansible 2.9.11.

### Installation
1) Prepare vagrant environment

2) Run:
```sh
ansible-playbook main.yml
```

### Advanced
Install PostgreSQL on db hosts:
```sh
ansible-playbook main.yml --tags "pg"
```

Install repmgr on db hosts + configure asynchronous replication using repmgr:
```sh
ansible-playbook main.yml --tags "repmgr"
```

### Vars
```sh
host_vars/vagrant1
host_vars/vagrant2
group_vars/databases
