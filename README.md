# Ansible: Standard setup for docker and docker-compose on ubuntu

This is an [Ansible](https://www.ansible.com) playbook to setup a single Ubuntu server with [Docker](https://www.docker.com) and [Docker-compose](https://docs.docker.com/compose/install/).

## Requirements

+ Ansible

## Tools

This playbook is designed to install a ubuntu server, add users, keys, configurations and add a bunch of useful tools:

+ [Docker](https://www.docker.com)
+ [Docker-compose](https://docs.docker.com/compose/install/)

## Installing on hcloud

Setup ansible to work with hcloud host
TODO add description

Copy pubkey from functional drone user to keys/drone.pubkey and functional debug user to keys/debug.pubkey

Copy the hosts example file and change the values to your needs:

```bash
$ cp hosts.example hosts
```

Setup your variables in the `playbook.yml` file.

Then run the playbook:

```bash
$ ansible-playbook -i hosts playbook.yml
```

## License

This project is released under the [MIT](http://opensource.org/licenses/MIT) license.