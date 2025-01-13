#Ansible роли для запуска Joomla для Ubuntu 20.04
Роли:
  - nginx
  - mysql
  - php
  - joomla
#Команда для запуска плейбука
ansible-playbook -i inventory.yml playbook.yml -e secret.vault --vault-password-file password_vault.txt

