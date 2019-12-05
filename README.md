docker_aws_instance
=========

This ansible role is to create an CentOS

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

No dependencies for this playbook

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
---
- hosts: localhost
  become: true
  gather_facts: false
  vars:
    keypair: hemanth
    instance_type: t2.micro
    security_group: sg-0fa454335a1f75b19
    image: ami-01ed306a12b7d1c96
    region: us-west-2
    ec2_access_key: ABCEFG
    ec2_secret_key: ABCEFG+XZ
  roles:
    - hemanth22.docker_aws_instance
```

License
-------

GPLv3

Author Information
------------------

This role was created in 2019 by Hemanth BITRA.
