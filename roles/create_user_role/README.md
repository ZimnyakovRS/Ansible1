Create_user
=========

Роль для создания пользователя и получения доступа к нему 
с помощью ключей

Role Variables
--------------


- user # Имя пользователя
- authorized_keys_list # список ключей для авторизации, 
по умолчанию есть два ключа

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
- name: Create user playbook
  hosts: all
  gather_facts: yes
  roles:
    - create_user_role
```

Author Information
------------------
- name: Zimnyakov Ruslan
- email: rzimnyakovwork@gmail.com