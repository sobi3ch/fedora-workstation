# Fedora Workstation

This is an opinionated playbook to setup a Fedora 32+ workstation with everything you need to start developing on Fedora Linux.

## Quick Setup

Follow these steps to install Ansible, checkout the Fedora Workstation repo, and run the playbook:

```
sudo dnf install ansible -y
git clone https://github.com/sobi3ch/fedora-workstation.git
cd fedora-workstation
ansible-playbook setup_workstation.yml -e "local_user=sobi3ch local_user_email=piotr.sobieszczanski@gmail.com" --become --ask-become-pass
```

For further customization, edit `vars/vars.yml` to fit your needs.
