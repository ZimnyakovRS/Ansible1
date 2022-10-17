# Если ssh-key запаролен
Нужно добавить пароль в ssh агента с помощью:
```
eval `ssh-agent -s`
ssh-add
```