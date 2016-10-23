Role Name
=========

Installation of bits from Docker, Inc. useful in running a Docker host.

Requirements
------------

TODO

Role Variables
--------------

* docker_engine_install: true
* docker_engine_graph: /var/lib/docker
* docker_engine_storage_driver: overlay2
* docker_engine_log_size: 1g
* docker_compose_install: true
* docker_compose_version: 1.8.1
* docker_machine_install: true
* docker_machine_version: 0.8.2

Dependencies
------------

No dependencies.

Example Playbook
----------------

```
- hosts: servers
  roles:
      - { role: kurron.docker-host, jvm_sdkman_install: false, vm_intellij_version: 2016.2.4, jvm_intellij_build: 162.2032.8 }
```

License
-------

This project is licensed under the [Apache License Version 2.0, January 2004](http://www.apache.org/licenses/).

Author Information
------------------

[Author's website](http://jvmguy.com/).
