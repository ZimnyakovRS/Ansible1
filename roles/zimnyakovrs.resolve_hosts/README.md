zimnyakovrs.resolve_hosts
=========
Правка /etc/hosts для резолва внутри локальной сети

Role Variables
--------------
host_list - список записей в файле hosts, находится в одноименном файле в role defaults (зашифрован)

Пример:
```yaml
host_list:
  - pattern: 192.168.0.10
    line: 192.168.0.50 HOST1 host1 host1.local
  - pattern: 192.168.0.20
    line: 192.168.0.1 HOST2 host2 host2.local
```
Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
- name: Play - change /etc/hosts
  hosts: all
  gather_facts: yes
  roles:
    - zimnyakovrs.resolve_hosts
```

Author Information
------------------
- name: Zimnyakov Ruslan
- email: rzimnyakovwork@gmail.com