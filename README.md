fouadsemaan.kubernetes-cluster
=========

Configures a Kubernetes cluster. Assumes you have a secured etcd cluster.

Requirements
------------

See [meta/main.yml](meta/main.yml)

Role Variables
--------------

See [defaults/main.yml](defaults/main.yml)

Dependencies
------------

See [meta/main.yml](meta/main.yml)

Example Playbook
----------------

inventory.ini
```ini
[etcd-master]
host1
host2
...

[kubernetes]
hostA
hostB
...
```

playbook.yml
```yml
- hosts: kubernetes
  roles:
    - fouadsemaan.kubernetes-cluster
```

License
-------

MIT

Author Information
------------------

Andrew Rothstein <andrew.rothstein@gmail.com>
Fouad Semaan <semaanfouad@gmail.com>
