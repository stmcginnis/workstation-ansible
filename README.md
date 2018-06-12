# Ansible Workstation Setup

This contains a set of Ansible tasks to easily set up a new
workstation with a set of expected packages installed and
some basic settings.

## Usage

This has been tested locally using Ansible 2.5 on Fedora, but
should theoretically work on Debian or Red Hat based distros.

This can be run by pulling from a remote git repo. One suggestion
is to fork this repo, then update all values in `host_vars/localhost`
for your specific settings. It can then be used by calling something
similar to:

```
sudo ansible-pull -U https://github.com/stmcginnis/workstation-ansible
```

Alternatively, you can clone this locally, update the variables, then
run:

```
sudo ansible-playbook local.yml
```

