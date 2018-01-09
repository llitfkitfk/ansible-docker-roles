# ansible docker roles



* `docker-setup` install docker (Support RedHat and Debian)
* `swarm-setup` install swarm mode cluster
* `docker-tls` enable docker tls

```
---
- name: Setup docker environment & swarm mode cluster & enable docker tls
  hosts: all
  roles:
    - role: docker-setup
    - role: swarm-setup
    - role: docker-tls
  tasks:

```