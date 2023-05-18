# ansible-role-update-package-manager-cache

[![molecule](https://github.com/diodonfrost/ansible-role-update-package-manager-cache/workflows/molecule/badge.svg)](https://github.com/diodonfrost/ansible-role-update-package-manager-cache/actions)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-diodonfrost.update_package_manager_cache-660198.svg)](https://galaxy.ansible.com/diodonfrost/update_package_manager_cache)

This role provide a compliance for install update_package_manager_cache on your target host.

## Requirements

This role was developed using Ansible 2.12 Backwards compatibility is not guaranteed.
Use `ansible-galaxy install diodonfrost.update_package_manager_cache` to install the role on your system.
*   Ansible >= 2.12

## Role Variables

This role has multiple variables. The defaults for all these variables are the following:

```yaml
---
# defaults file for ansible-role-update-package-manager-cache
```

## Dependencies

None

## Example Playbook

This is a sample playbook file for deploying the Ansible Galaxy update_package_manager_cache role in a localhost and installing the latest version of update_package_manager_cache.

```yaml
---
- hosts: localhost
  become: true
  roles:
    - role: diodonfrost.update_package_manager_cache
```

## Local Testing

This project uses [Molecule](http://molecule.readthedocs.io/) to aid in the
development and testing.

To develop or test you'll need to have installed the following:

* Linux (e.g. [Ubuntu](http://www.ubuntu.com/))
* [Docker](https://www.docker.com/)
* [Python](https://www.python.org/) (including python-pip)
* [Ansible](https://www.ansible.com/)
* [Molecule](http://molecule.readthedocs.io/)

### Testing with Docker

```shell
# Install requirements
pip install -r requirements-dev.txt

# Test ansible role with ubuntu 22.04
molecule test

# Test ansible role with alpine latest
image=ansible-fedora:38 molecule test

# Create fedora 38 instance
image=ansible-fedora:38 molecule create

# Apply role on fedora instance
image=ansible-fedora:38 molecule converge

# Launch tests on fedora instance
image=ansible-fedora:38 molecule verify
```

## License

Apache 2

## Author Information

This role was created in 2023 by diodonfrost.
