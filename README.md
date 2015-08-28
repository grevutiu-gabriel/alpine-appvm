# Alpine-based AppVMs for QEMU

This is a playbook that helps you create AppVMs using Alpine Linux. Right now,
only QEMU is supposed with SPICE enabled, but support for other environments
may be added in the future.

## Prerequisites
* [ansible](https://github.com/ansible/ansible) 2.0+ (build from git for now)
* An existing Alpine Linux install; you can use the provided setup-alpine.conf
  to help with this. Simply call `setup-alpine -f setup-alpine.conf` after
  copying the file over.

## Usage
* Create an inventory file. Follow the [Ansible
  documentation](http://docs.ansible.com) for help with this. You will need to
  define, at minimum, a user variable for the host.
* Copy example.yml to a new file and modify as desired.
* Run the playbook using ansible-playbook.