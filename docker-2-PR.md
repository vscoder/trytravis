# Выполнено ДЗ №12

 - [x] Основное ДЗ
 - [x] Задание со *

## В процессе сделано:

### Подготовка репозитория. Основы работы с docker
- Создан репозиторий
- Выполнена интеграция репозитория со slack
- Настроены уведомления в slack от travis-ci
- Создан Makefile
- Установлены: docker, docker-compose, docker-machine
- Описаны основные команды docker

### Задание со *: Отличия образа и контейнера
- В README.md добавлены ссылки по теме
- Произведён анализ результатов вывода команды docker inspect <u_image_id>
- Произведён анализ вывода команды docker inspect <u_container_id>
- В файле docker-monolith/docker-1.log описаны различия между образом и контейнером

### Docker контейнеры
- Создан новый проект в GCE
- Описана работа с Docker machine
- Настроена работа docker machine с инстансом в GCE
- **Подробно** описаны особенности работы docker с namespaces, включая некоторые эксперименты:
  - PID namespace
  - NET namespace
  - USER namespace
- Создан Dockerfile для упаковки reddit-app и MongoDB в контейнер
- Из Dockerfile создан образ
- Из образа создан и запущен контейнер

### Docker hub
- Образ загружен на docker-hub
- Выполнен вход на https://hub.docker.com/
- Выполнена авторизация docker на dockerhub docker login
- docker-образ загружен на докер хаб
- Образ скачан с docker-hub и запущен на локальной машине
- Выполнено множество проверок

### Задание со *: IaC с использованием docker
#### Packer
- Подготовлены необходимые цели в Makefile.
- Создан шаблон packer и скрипт-обёртка для подготовки базового образа
- Создан ansible-playbook docker.yml для провиженинга packer-образа. Использована galaxy-роль geerlingguy.docker
- Созданы необходимые для работы ansible файлы
- Средствами packer подготовлен базовый образ make monolith_packer_build

#### Terraform
- Создан bucket для хранения состояния terraform
- Настроен projeckt-wide ssh ключ
- Создан модуль instance, описывающий абстрактный Goocle Compute Instance
- Создана stage-инфраструктура. Особенности:
  - Количество инстансов берётся из переменной docker_app_instance_count
  - Префикс имени инстанса docker_app_name_prefix
  - Список тегов docker_app_tags
  - Список tcp-портов для фаервола docker_app_tcp_ports

#### Запуск контейнера средствами ansible
- Создана роль docker-monolith/ansible/roles/reddit-monolith-docker
- Настроено использование динамического инвентори gcp_compute
- Зависимости requirements.yml перемещены в docker-monolith/ansible/environments/stage/requirements.yml
- В docker-monolith/terraform/modules/instance/main.tf добавлены labels к google_compute_instance
- Добавлен плейбук reddit-app.yml для деплоя контейнера

#### Автоматизированное тестирование travis-ci
- `trytravis` установлен и добавлен в [requirements-dev.txt](requirements-dev.txt)
- Добавлены тесты средствами travis-ci
  - `monolith_packer_validate` 
  - `monolith_terraform_validate` 
  - `monolith_terraform_tflint`
  - `monolith_ansible_syntax` 
  - `monolith_ansible_lint`

### Прочее/вне заданий
- В README.md добавлено оглавление
- В README.md добавлен статус тестов на travis-ci
- В README.md добавлен TODO по улучшению безопасности docker-демона и запускаемого контейнера. Добавлен ряд заметок и ссылок по теме.
- Добавлен результат выполнения docker-bench-security

## Как запустить проект:
- Установить ansible и необходимые пакеты `make install_requirements`
- При необходимости, установить docker-machine `make install_docker_machine`
- Установить packer и terraform `make install_packer install_terraform install_tflint`
- Установить внешние ansible-роли `make monolith_ansible_install_requirements`
- Заполнить переменные packer [docker-monolith/packer/variables.json](docker-monolith/packer/variables.json)
- Собрать packer базовый образ `make monolith_packer_build`
- Инициализировать базовую terraform инфраструктуру `make monolith_terraform_init ENV=""`
- Инициализировать terraform инфраструктуру stage `make monolith_terraform_init ENV="stage"`
- Заполнить переменные terraform [docker-monolith/terraform/terraform.tfvars](docker-monolith/terraform/terraform.tfvars) и [docker-monolith/terraform/stage/terraform.tfvars](docker-monolith/terraform/stage/terraform.tfvars)
- Создать bucket для хранения стейта `make monolith_terraform_apply ENV=""`
- Создать stage инфраструктуру `make monolith_terraform_apply ENV="stage"`
- Залогиниться на docker hub `docker login`
- Собрать и загрузить на docker-hub образ с приложением `make monolith_docker_build monolith_docker_publish`
- Запустить образ `make monolith_ansible_reddit_app`

## Как проверить работоспособность:
- Открыть в браузере http://<instance ip>:9292, где instance ip это любой из ip-адресов, отображённых при создании инфраструктуры `make monolith_terraform_apply`

## PR checklist
 - [x] Выставил label с номером домашнего задания
 - [x] Выставил label с темой домашнего задания
