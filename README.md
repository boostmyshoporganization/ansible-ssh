Ansible Ssh
==============

Install and configure ssh on Debian server.

Installation
------------

git submodule add git@github.com/boostmyshoporganization/ansible-ssh roles/ssh

```yaml
roles:
    - ssh
```

Configuration
-------------

```yaml
ssh:
  port: 22
  public_keys:
    - { user: 'root', path: './files/ssh/public_keys/gdievart' }
    - { user: 'root', path: './files/ssh/public_keys/jenkins' }
```