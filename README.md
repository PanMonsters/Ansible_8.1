# Самоконтроль выполненения задания

1. Где расположен файл с `some_fact` из второго пункта задания?  
Ответ:  
/group_vars/all/examp.yml  

2. Какая команда нужна для запуска вашего `playbook` на окружении `test.yml`?  
Ответ:  
ansible-playbook -i inventory/test.yml site.yml  

3. Какой командой можно зашифровать файл?  
Ответ:  
ansible-vault encrypt <file>  

4. Какой командой можно расшифровать файл?  
Ответ:  
ansible-vault decrypt <file>  

5. Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?  
Ответ:  
ansible-vault view

6. Как выглядит команда запуска `playbook`, если переменные зашифрованы?  
Ответ:  
ansible-playbook -i inventory/prod.yml site.yml --ask-vault-pass  

7. Как называется модуль подключения к host на windows?  
Ответ:  
[winrm](https://docs.ansible.com/ansible/latest/user_guide/windows_winrm.html)  
[psrp](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/psrp_connection.html)  

8. Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh  
Ответ:  
ansible-doc -t connection ssh  

9. Какой параметр из модуля подключения `ssh` необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?  
Ответ:  
remote_user  
