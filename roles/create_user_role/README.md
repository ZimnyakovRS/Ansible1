Create_user
=========

Роль для создания пользователя и получения доступа к нему 
с помощью ключей

Role Variables
--------------


- `user` - Имя пользователя
- `user_fio` - Комментарий к создаваемому пользователю.
- `authorized_keys_list` - список ключей для авторизации, 
по умолчанию есть два ключа. 
Находится в `defaults/main/auth_keys_enc.yml`, который зашифрован.

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
- `Zimnyakov Ruslan`
- `rzimnyakovwork@gmail.com`