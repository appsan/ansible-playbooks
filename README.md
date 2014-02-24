ansible-playbooks
=================

Ansible playbooks for Ubuntu

## Requirements

* Ansible
* Python 2.6 

See [guide](http://docs.ansible.com/intro_installation.html) on how to setup Ansible.

## Usage

Basic:

```
$ ansible-playbook -i hosts site.yml
```

With SSH key:

```
$ ansible-playbook -i hosts site.yml --private-key=mysshkey.pem
```

Run on single target without source file:

```
ansible-playbook -i "example.com," site.yml
```

To ignore SSH host key check, do
```
$ export ANSIBLE_HOST_KEY_CHECKING=False
```

