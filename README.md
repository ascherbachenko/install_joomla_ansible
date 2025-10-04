# Роль установки Joomla
1. Для установки скачайте удаленный репозиторий командой
```bash
git clone https://github.com/ascherbachenko/install_joomla_ansible
```
2. Выполните внутри каталога команду:
```bash
ansible-playbook -i invenroty/linux.yaml install_cms.yaml --ask-vault-pass
```
3. Для расшифровки переменных используется пароль `12345678`
> Примечание: 
Если после первой установки, будет повторная установка mysql, нужно в задании  `Change password root user in MySQL` закомментировать строку с `login_unix_socket` и раскомментировать строки `login_user`, `login_password`