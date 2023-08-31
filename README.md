ansible-system-role
=========

Ansible role to perform basic system setup incl. Docker, /etc/hosts management and swap management

Requirements
------------

None

Role Variables
--------------
```YAML
---
# Enable the system role
system_defaults_enabled: false

# Install or update latest packages
system_package_mode: present

# Basic required system packages
system_packages: []

# Additional packages to be installed on the systems
system_additional_packages: []

# Apply the grub optimisations (elevate)
system_optimize_grub: false

# Grub elevator mode: 'noop' for VMGUESTS or 'deadline' for VMHOSTS
system_grub_elevator_mode: ""

# Deploy etc hosts
system_etc_hosts: false

# Add entries to /etc/hosts (note: will REPLACE the whole /etc/hosts file)
system_etc_hosts_list: []
# - host: example.tld
#   ip: 1.2.3.4

# Setup Docker
system_docker_setup: false

# User group for docker users
system_docker_group: docker

# Add docker user to docker group
system_docker_user: ""

# Disable swap on server
system_swap_disable: false

# Remove swap files
system_swap_remove_files: true
```

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: methorz.system }

License
-------

BSD

Author Information
------------------

https://twitter.com/methor_z
