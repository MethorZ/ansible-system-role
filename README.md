ansible-system-role
=========

Ansible role to perform basic system setup

Requirements
------------

None

Role Variables
--------------
```YAML
# Install or update latest packages
system_package_mode: latest # present

# Additional packages to be installed on the systems
system_additional_packages: []

```

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: methorz.ansible-system-role }

License
-------

BSD

Author Information
------------------

https://twitter.com/methor_z
