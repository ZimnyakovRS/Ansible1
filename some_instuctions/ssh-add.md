# Если ssh-key запаролен
Нужно добавить пароль в ssh агента с помощью:
```
cd ~
ssh-agent bash
ssh-add .ssh/id_rsa
```