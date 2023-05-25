Ansible Role Prometheus - Node Exporter
=========

This role installs and configures Prometheus Node Exporter on Ubuntu 20.04+.

Requirements
------------

Operating System Support: Ubuntu 20.04 or later

Role Variables
--------------

# Security
```
# pmh_node_exporter_basic_auth_key: node_exporter
pmh_node_exporter_service_user: node_exporter
# pmh_node_exporter_prometheus_server_ip_addresses:
#   - 0.0.0.0/0
```

# Package Management
```
# pmh_node_exporter_package_version: 1.5.0
# pmh_node_exporter_package_os_arch: amd64
```

Dependencies
------------

No dependency.

Example Playbook
----------------

Install
```
ansible-galaxy install cihanyilmazer.ansible_role_prometheus
```

    - hosts: servers
      roles:
         - cihanyilmazer.ansible_role_prometheus/node_exporter

License
-------

MIT

Author Information
------------------

Cihan Yilmazer<br />
https://www.cihanyilmazer.com<br />
https://www.github.com/cihanyilmazer<br />
https://galaxy.ansible.com/cihanyilmazer<br />