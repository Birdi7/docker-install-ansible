# Что делает?
Устанавливает docker & docker-compose на Ubuntu сервер через ssh.

# Как юзать?
1. Добавь свой ssh key на сервер
2. Установи себе ансибл `brew install ansible`
3. Поменяй в [provisioning/hosts.yml](provisioning/hosts.yml) переменную `ansible_host` на идентификатор твоего сервера
4. Запусти `ansible-playbook provisioning/site.yml -i provisioning/hosts.yml`
5. Радуйся
