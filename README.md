# Ansible роли для запуска Joomla для Ubuntu 20.04

## Роли:
  - nginx
  - mysql
  - php
  - joomla

# Версии используемых сервисов:
- nginx 1.18.0
- mysql-server-8.0.40-0ubuntu0.20.04.1
- php 8.1
- joomla 5.1.4

# Переменные
## Для подключения к хосту, просто указать значения переменных в playbook.yml:
- ans_host:
- ans_user:
- ans_password
  
# Команда для запуска плейбука:
`ansible-playbook -i inventory.yml playbook.yml -e secret.vault --vault-password-file password_vault.txt`

# Пароль для Ansible-vaul:
Находится в файле password_vault.txt
### В Ansible-vaul находятся пароли к mysql пользователя root и admin.
