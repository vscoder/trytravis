# vscoder_infra
Aleksey Koloskov OTUS-DevOps-2019-08 Infra repository

[![Build Status](https://travis-ci.com/Otus-DevOps-2019-08/vscoder_infra.svg?branch=master)](https://travis-ci.com/Otus-DevOps-2019-08/vscoder_infra)

- [vscoder_infra](#vscoderinfra)
- [Домашние задания](#%d0%94%d0%be%d0%bc%d0%b0%d1%88%d0%bd%d0%b8%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d1%8f)
  - [HomeWork 2: GitChatOps](#homework-2-gitchatops)
  - [HomeWork 3: Знакомство с облачной инфраструктурой. Google Cloud Platform](#homework-3-%d0%97%d0%bd%d0%b0%d0%ba%d0%be%d0%bc%d1%81%d1%82%d0%b2%d0%be-%d1%81-%d0%be%d0%b1%d0%bb%d0%b0%d1%87%d0%bd%d0%be%d0%b9-%d0%b8%d0%bd%d1%84%d1%80%d0%b0%d1%81%d1%82%d1%80%d1%83%d0%ba%d1%82%d1%83%d1%80%d0%be%d0%b9-google-cloud-platform)
  - [HomeWork 4: Деплой тестового приложения](#homework-4-%d0%94%d0%b5%d0%bf%d0%bb%d0%be%d0%b9-%d1%82%d0%b5%d1%81%d1%82%d0%be%d0%b2%d0%be%d0%b3%d0%be-%d0%bf%d1%80%d0%b8%d0%bb%d0%be%d0%b6%d0%b5%d0%bd%d0%b8%d1%8f)
    - [Основное задание](#%d0%9e%d1%81%d0%bd%d0%be%d0%b2%d0%bd%d0%be%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5)
    - [Самостоятельная работа](#%d0%a1%d0%b0%d0%bc%d0%be%d1%81%d1%82%d0%be%d1%8f%d1%82%d0%b5%d0%bb%d1%8c%d0%bd%d0%b0%d1%8f-%d1%80%d0%b0%d0%b1%d0%be%d1%82%d0%b0)
    - [Дополнительное задание 1](#%d0%94%d0%be%d0%bf%d0%be%d0%bb%d0%bd%d0%b8%d1%82%d0%b5%d0%bb%d1%8c%d0%bd%d0%be%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-1)
    - [Дополнительное задание 2](#%d0%94%d0%be%d0%bf%d0%be%d0%bb%d0%bd%d0%b8%d1%82%d0%b5%d0%bb%d1%8c%d0%bd%d0%be%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-2)
    - [Прочее](#%d0%9f%d1%80%d0%be%d1%87%d0%b5%d0%b5)
  - [HomeWork 5: Сборка образов VM при помощи Paker](#homework-5-%d0%a1%d0%b1%d0%be%d1%80%d0%ba%d0%b0-%d0%be%d0%b1%d1%80%d0%b0%d0%b7%d0%be%d0%b2-vm-%d0%bf%d1%80%d0%b8-%d0%bf%d0%be%d0%bc%d0%be%d1%89%d0%b8-paker)
    - [Основное задание](#%d0%9e%d1%81%d0%bd%d0%be%d0%b2%d0%bd%d0%be%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-1)
    - [Самостоятельные задания](#%d0%a1%d0%b0%d0%bc%d0%be%d1%81%d1%82%d0%be%d1%8f%d1%82%d0%b5%d0%bb%d1%8c%d0%bd%d1%8b%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d1%8f)
    - [Первое задание со *](#%d0%9f%d0%b5%d1%80%d0%b2%d0%be%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-%d1%81%d0%be)
    - [Второе задание со *](#%d0%92%d1%82%d0%be%d1%80%d0%be%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-%d1%81%d0%be)
  - [HomeWork 6: Практика IaC с использованием Terraform](#homework-6-%d0%9f%d1%80%d0%b0%d0%ba%d1%82%d0%b8%d0%ba%d0%b0-iac-%d1%81-%d0%b8%d1%81%d0%bf%d0%be%d0%bb%d1%8c%d0%b7%d0%be%d0%b2%d0%b0%d0%bd%d0%b8%d0%b5%d0%bc-terraform)
    - [Основное задание](#%d0%9e%d1%81%d0%bd%d0%be%d0%b2%d0%bd%d0%be%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-2)
    - [Самостоятельные задания](#%d0%a1%d0%b0%d0%bc%d0%be%d1%81%d1%82%d0%be%d1%8f%d1%82%d0%b5%d0%bb%d1%8c%d0%bd%d1%8b%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d1%8f-1)
    - [Задания со *](#%d0%97%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d1%8f-%d1%81%d0%be)
    - [Задания с **](#%d0%97%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d1%8f-%d1%81)
  - [HomeWork 7: Принципы организации инфраструктурного кода и работа над инфраструктурой в команде на примере Terraform](#homework-7-%d0%9f%d1%80%d0%b8%d0%bd%d1%86%d0%b8%d0%bf%d1%8b-%d0%be%d1%80%d0%b3%d0%b0%d0%bd%d0%b8%d0%b7%d0%b0%d1%86%d0%b8%d0%b8-%d0%b8%d0%bd%d1%84%d1%80%d0%b0%d1%81%d1%82%d1%80%d1%83%d0%ba%d1%82%d1%83%d1%80%d0%bd%d0%be%d0%b3%d0%be-%d0%ba%d0%be%d0%b4%d0%b0-%d0%b8-%d1%80%d0%b0%d0%b1%d0%be%d1%82%d0%b0-%d0%bd%d0%b0%d0%b4-%d0%b8%d0%bd%d1%84%d1%80%d0%b0%d1%81%d1%82%d1%80%d1%83%d0%ba%d1%82%d1%83%d1%80%d0%be%d0%b9-%d0%b2-%d0%ba%d0%be%d0%bc%d0%b0%d0%bd%d0%b4%d0%b5-%d0%bd%d0%b0-%d0%bf%d1%80%d0%b8%d0%bc%d0%b5%d1%80%d0%b5-terraform)
    - [Основное задание](#%d0%9e%d1%81%d0%bd%d0%be%d0%b2%d0%bd%d0%be%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-3)
    - [Задания со * Хранение state в gcs](#%d0%97%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d1%8f-%d1%81%d0%be--%d0%a5%d1%80%d0%b0%d0%bd%d0%b5%d0%bd%d0%b8%d0%b5-state-%d0%b2-gcs)
    - [Задание с ** Провиженинг приложения с использованием пременных окружения](#%d0%97%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-%d1%81--%d0%9f%d1%80%d0%be%d0%b2%d0%b8%d0%b6%d0%b5%d0%bd%d0%b8%d0%bd%d0%b3-%d0%bf%d1%80%d0%b8%d0%bb%d0%be%d0%b6%d0%b5%d0%bd%d0%b8%d1%8f-%d1%81-%d0%b8%d1%81%d0%bf%d0%be%d0%bb%d1%8c%d0%b7%d0%be%d0%b2%d0%b0%d0%bd%d0%b8%d0%b5%d0%bc-%d0%bf%d1%80%d0%b5%d0%bc%d0%b5%d0%bd%d0%bd%d1%8b%d1%85-%d0%be%d0%ba%d1%80%d1%83%d0%b6%d0%b5%d0%bd%d0%b8%d1%8f)
  - [HomeWork 8: Управление конфигурацией. Основные DevOps инструменты. Знакомство с Ansible](#homework-8-%d0%a3%d0%bf%d1%80%d0%b0%d0%b2%d0%bb%d0%b5%d0%bd%d0%b8%d0%b5-%d0%ba%d0%be%d0%bd%d1%84%d0%b8%d0%b3%d1%83%d1%80%d0%b0%d1%86%d0%b8%d0%b5%d0%b9-%d0%9e%d1%81%d0%bd%d0%be%d0%b2%d0%bd%d1%8b%d0%b5-devops-%d0%b8%d0%bd%d1%81%d1%82%d1%80%d1%83%d0%bc%d0%b5%d0%bd%d1%82%d1%8b-%d0%97%d0%bd%d0%b0%d0%ba%d0%be%d0%bc%d1%81%d1%82%d0%b2%d0%be-%d1%81-ansible)
    - [Основное задание](#%d0%9e%d1%81%d0%bd%d0%be%d0%b2%d0%bd%d0%be%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-4)
    - [Задание со \*: Работа с динамическим inventory](#%d0%97%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-%d1%81%d0%be--%d0%a0%d0%b0%d0%b1%d0%be%d1%82%d0%b0-%d1%81-%d0%b4%d0%b8%d0%bd%d0%b0%d0%bc%d0%b8%d1%87%d0%b5%d1%81%d0%ba%d0%b8%d0%bc-inventory)
  - [HomeWork 9: Деплой и управление конфигурацией с Ansible](#homework-9-%d0%94%d0%b5%d0%bf%d0%bb%d0%be%d0%b9-%d0%b8-%d1%83%d0%bf%d1%80%d0%b0%d0%b2%d0%bb%d0%b5%d0%bd%d0%b8%d0%b5-%d0%ba%d0%be%d0%bd%d1%84%d0%b8%d0%b3%d1%83%d1%80%d0%b0%d1%86%d0%b8%d0%b5%d0%b9-%d1%81-ansible)
    - [Основное задание](#%d0%9e%d1%81%d0%bd%d0%be%d0%b2%d0%bd%d0%be%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-5)
  - [* Закомментирован провиженинг приложения средствами terraform](#%d0%97%d0%b0%d0%ba%d0%be%d0%bc%d0%bc%d0%b5%d0%bd%d1%82%d0%b8%d1%80%d0%be%d0%b2%d0%b0%d0%bd-%d0%bf%d1%80%d0%be%d0%b2%d0%b8%d0%b6%d0%b5%d0%bd%d0%b8%d0%bd%d0%b3-%d0%bf%d1%80%d0%b8%d0%bb%d0%be%d0%b6%d0%b5%d0%bd%d0%b8%d1%8f-%d1%81%d1%80%d0%b5%d0%b4%d1%81%d1%82%d0%b2%d0%b0%d0%bc%d0%b8-terraform)
  - [* К задаче добавлена секция `notify`, которая сообщает о необходимости запуска хендлера.](#%d0%9a-%d0%b7%d0%b0%d0%b4%d0%b0%d1%87%d0%b5-%d0%b4%d0%be%d0%b1%d0%b0%d0%b2%d0%bb%d0%b5%d0%bd%d0%b0-%d1%81%d0%b5%d0%ba%d1%86%d0%b8%d1%8f-notify-%d0%ba%d0%be%d1%82%d0%be%d1%80%d0%b0%d1%8f-%d1%81%d0%be%d0%be%d0%b1%d1%89%d0%b0%d0%b5%d1%82-%d0%be-%d0%bd%d0%b5%d0%be%d0%b1%d1%85%d0%be%d0%b4%d0%b8%d0%bc%d0%be%d1%81%d1%82%d0%b8-%d0%b7%d0%b0%d0%bf%d1%83%d1%81%d0%ba%d0%b0-%d1%85%d0%b5%d0%bd%d0%b4%d0%bb%d0%b5%d1%80%d0%b0)
  - [* Добавлена задача по установке зависимостей, модуль `bundler`](#%d0%94%d0%be%d0%b1%d0%b0%d0%b2%d0%bb%d0%b5%d0%bd%d0%b0-%d0%b7%d0%b0%d0%b4%d0%b0%d1%87%d0%b0-%d0%bf%d0%be-%d1%83%d1%81%d1%82%d0%b0%d0%bd%d0%be%d0%b2%d0%ba%d0%b5-%d0%b7%d0%b0%d0%b2%d0%b8%d1%81%d0%b8%d0%bc%d0%be%d1%81%d1%82%d0%b5%d0%b9-%d0%bc%d0%be%d0%b4%d1%83%d0%bb%d1%8c-bundler)
  - [* В плейбук добавлен сценарий `Deploy App` с тегом `deploy-tag` для деплоя приложения](#%d0%92-%d0%bf%d0%bb%d0%b5%d0%b9%d0%b1%d1%83%d0%ba-%d0%b4%d0%be%d0%b1%d0%b0%d0%b2%d0%bb%d0%b5%d0%bd-%d1%81%d1%86%d0%b5%d0%bd%d0%b0%d1%80%d0%b8%d0%b9-deploy-app-%d1%81-%d1%82%d0%b5%d0%b3%d0%be%d0%bc-deploy-tag-%d0%b4%d0%bb%d1%8f-%d0%b4%d0%b5%d0%bf%d0%bb%d0%be%d1%8f-%d0%bf%d1%80%d0%b8%d0%bb%d0%be%d0%b6%d0%b5%d0%bd%d0%b8%d1%8f)
    - [Задание со \*: Динамический inventory](#%d0%97%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-%d1%81%d0%be--%d0%94%d0%b8%d0%bd%d0%b0%d0%bc%d0%b8%d1%87%d0%b5%d1%81%d0%ba%d0%b8%d0%b9-inventory)
      - [Исследование](#%d0%98%d1%81%d1%81%d0%bb%d0%b5%d0%b4%d0%be%d0%b2%d0%b0%d0%bd%d0%b8%d0%b5)
      - [Реализация](#%d0%a0%d0%b5%d0%b0%d0%bb%d0%b8%d0%b7%d0%b0%d1%86%d0%b8%d1%8f)
    - [Провижининг в Packer](#%d0%9f%d1%80%d0%be%d0%b2%d0%b8%d0%b6%d0%b8%d0%bd%d0%b8%d0%bd%d0%b3-%d0%b2-packer)
    - [Вне задания: Makefile](#%d0%92%d0%bd%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d1%8f-makefile)
  - [HomeWork 10: Ansible: работа с ролями и окружениями](#homework-10-ansible-%d1%80%d0%b0%d0%b1%d0%be%d1%82%d0%b0-%d1%81-%d1%80%d0%be%d0%bb%d1%8f%d0%bc%d0%b8-%d0%b8-%d0%be%d0%ba%d1%80%d1%83%d0%b6%d0%b5%d0%bd%d0%b8%d1%8f%d0%bc%d0%b8)
    - [Основное задание](#%d0%9e%d1%81%d0%bd%d0%be%d0%b2%d0%bd%d0%be%d0%b5-%d0%b7%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-6)
      - [Роль db](#%d0%a0%d0%be%d0%bb%d1%8c-db)
      - [Роль app](#%d0%a0%d0%be%d0%bb%d1%8c-app)
      - [Плейбуки для app и db](#%d0%9f%d0%bb%d0%b5%d0%b9%d0%b1%d1%83%d0%ba%d0%b8-%d0%b4%d0%bb%d1%8f-app-%d0%b8-db)
      - [Окружения](#%d0%9e%d0%ba%d1%80%d1%83%d0%b6%d0%b5%d0%bd%d0%b8%d1%8f)
      - [Проверка](#%d0%9f%d1%80%d0%be%d0%b2%d0%b5%d1%80%d0%ba%d0%b0)
      - [Работа с Community-ролями](#%d0%a0%d0%b0%d0%b1%d0%be%d1%82%d0%b0-%d1%81-community-%d1%80%d0%be%d0%bb%d1%8f%d0%bc%d0%b8)
      - [Ansible vault](#ansible-vault)
    - [Задание со \*: Использование динамического инвернтаря](#%d0%97%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-%d1%81%d0%be--%d0%98%d1%81%d0%bf%d0%be%d0%bb%d1%8c%d0%b7%d0%be%d0%b2%d0%b0%d0%bd%d0%b8%d0%b5-%d0%b4%d0%b8%d0%bd%d0%b0%d0%bc%d0%b8%d1%87%d0%b5%d1%81%d0%ba%d0%be%d0%b3%d0%be-%d0%b8%d0%bd%d0%b2%d0%b5%d1%80%d0%bd%d1%82%d0%b0%d1%80%d1%8f)
    - [Задание с \*\*: Настройка TravisCI](#%d0%97%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-%d1%81--%d0%9d%d0%b0%d1%81%d1%82%d1%80%d0%be%d0%b9%d0%ba%d0%b0-travisci)
      - [Подготовка](#%d0%9f%d0%be%d0%b4%d0%b3%d0%be%d1%82%d0%be%d0%b2%d0%ba%d0%b0)
      - [Trytravis](#trytravis)
      - [Реализация](#%d0%a0%d0%b5%d0%b0%d0%bb%d0%b8%d0%b7%d0%b0%d1%86%d0%b8%d1%8f-1)
  - [HomeWork 11: Разработка и тестирование Ansible ролей и плейбуков](#homework-11-%d0%a0%d0%b0%d0%b7%d1%80%d0%b0%d0%b1%d0%be%d1%82%d0%ba%d0%b0-%d0%b8-%d1%82%d0%b5%d1%81%d1%82%d0%b8%d1%80%d0%be%d0%b2%d0%b0%d0%bd%d0%b8%d0%b5-ansible-%d1%80%d0%be%d0%bb%d0%b5%d0%b9-%d0%b8-%d0%bf%d0%bb%d0%b5%d0%b9%d0%b1%d1%83%d0%ba%d0%be%d0%b2)
    - [Локальная разработка при помощи Vagrant, доработка ролей для провижининга в Vagrant](#%d0%9b%d0%be%d0%ba%d0%b0%d0%bb%d1%8c%d0%bd%d0%b0%d1%8f-%d1%80%d0%b0%d0%b7%d1%80%d0%b0%d0%b1%d0%be%d1%82%d0%ba%d0%b0-%d0%bf%d1%80%d0%b8-%d0%bf%d0%be%d0%bc%d0%be%d1%89%d0%b8-vagrant-%d0%b4%d0%be%d1%80%d0%b0%d0%b1%d0%be%d1%82%d0%ba%d0%b0-%d1%80%d0%be%d0%bb%d0%b5%d0%b9-%d0%b4%d0%bb%d1%8f-%d0%bf%d1%80%d0%be%d0%b2%d0%b8%d0%b6%d0%b8%d0%bd%d0%b8%d0%bd%d0%b3%d0%b0-%d0%b2-vagrant)
      - [Установка Vagrant](#%d0%a3%d1%81%d1%82%d0%b0%d0%bd%d0%be%d0%b2%d0%ba%d0%b0-vagrant)
      - [Доработка ролей](#%d0%94%d0%be%d1%80%d0%b0%d0%b1%d0%be%d1%82%d0%ba%d0%b0-%d1%80%d0%be%d0%bb%d0%b5%d0%b9)
        - [Provisioning](#provisioning)
      - [Задание со \*: Прлксирование средствами nginx](#%d0%97%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-%d1%81%d0%be--%d0%9f%d1%80%d0%bb%d0%ba%d1%81%d0%b8%d1%80%d0%be%d0%b2%d0%b0%d0%bd%d0%b8%d0%b5-%d1%81%d1%80%d0%b5%d0%b4%d1%81%d1%82%d0%b2%d0%b0%d0%bc%d0%b8-nginx)
        - [Исследование](#%d0%98%d1%81%d1%81%d0%bb%d0%b5%d0%b4%d0%be%d0%b2%d0%b0%d0%bd%d0%b8%d0%b5-1)
        - [Реализация](#%d0%a0%d0%b5%d0%b0%d0%bb%d0%b8%d0%b7%d0%b0%d1%86%d0%b8%d1%8f-2)
    - [Тестирование ролей при помощи Molecule и Testinfra](#%d0%a2%d0%b5%d1%81%d1%82%d0%b8%d1%80%d0%be%d0%b2%d0%b0%d0%bd%d0%b8%d0%b5-%d1%80%d0%be%d0%bb%d0%b5%d0%b9-%d0%bf%d1%80%d0%b8-%d0%bf%d0%be%d0%bc%d0%be%d1%89%d0%b8-molecule-%d0%b8-testinfra)
    - [Переключение сбора образов пакером на использование ролей](#%d0%9f%d0%b5%d1%80%d0%b5%d0%ba%d0%bb%d1%8e%d1%87%d0%b5%d0%bd%d0%b8%d0%b5-%d1%81%d0%b1%d0%be%d1%80%d0%b0-%d0%be%d0%b1%d1%80%d0%b0%d0%b7%d0%be%d0%b2-%d0%bf%d0%b0%d0%ba%d0%b5%d1%80%d0%be%d0%bc-%d0%bd%d0%b0-%d0%b8%d1%81%d0%bf%d0%be%d0%bb%d1%8c%d0%b7%d0%be%d0%b2%d0%b0%d0%bd%d0%b8%d0%b5-%d1%80%d0%be%d0%bb%d0%b5%d0%b9)
      - [Провиженинг в db.json](#%d0%9f%d1%80%d0%be%d0%b2%d0%b8%d0%b6%d0%b5%d0%bd%d0%b8%d0%bd%d0%b3-%d0%b2-dbjson)
      - [Провиженинг в app.json](#%d0%9f%d1%80%d0%be%d0%b2%d0%b8%d0%b6%d0%b5%d0%bd%d0%b8%d0%bd%d0%b3-%d0%b2-appjson)
    - [Задание со \*: Подключение Travis CI для автоматического прогона тестов](#%d0%97%d0%b0%d0%b4%d0%b0%d0%bd%d0%b8%d0%b5-%d1%81%d0%be--%d0%9f%d0%be%d0%b4%d0%ba%d0%bb%d1%8e%d1%87%d0%b5%d0%bd%d0%b8%d0%b5-travis-ci-%d0%b4%d0%bb%d1%8f-%d0%b0%d0%b2%d1%82%d0%be%d0%bc%d0%b0%d1%82%d0%b8%d1%87%d0%b5%d1%81%d0%ba%d0%be%d0%b3%d0%be-%d0%bf%d1%80%d0%be%d0%b3%d0%be%d0%bd%d0%b0-%d1%82%d0%b5%d1%81%d1%82%d0%be%d0%b2)
      - [Вынесение роли в отдельный репозиторий](#%d0%92%d1%8b%d0%bd%d0%b5%d1%81%d0%b5%d0%bd%d0%b8%d0%b5-%d1%80%d0%be%d0%bb%d0%b8-%d0%b2-%d0%be%d1%82%d0%b4%d0%b5%d0%bb%d1%8c%d0%bd%d1%8b%d0%b9-%d1%80%d0%b5%d0%bf%d0%be%d0%b7%d0%b8%d1%82%d0%be%d1%80%d0%b8%d0%b9)
        - [Подготовка репозитория](#%d0%9f%d0%be%d0%b4%d0%b3%d0%be%d1%82%d0%be%d0%b2%d0%ba%d0%b0-%d1%80%d0%b5%d0%bf%d0%be%d0%b7%d0%b8%d1%82%d0%be%d1%80%d0%b8%d1%8f)
        - [Переход на использование внешней роли](#%d0%9f%d0%b5%d1%80%d0%b5%d1%85%d0%be%d0%b4-%d0%bd%d0%b0-%d0%b8%d1%81%d0%bf%d0%be%d0%bb%d1%8c%d0%b7%d0%be%d0%b2%d0%b0%d0%bd%d0%b8%d0%b5-%d0%b2%d0%bd%d0%b5%d1%88%d0%bd%d0%b5%d0%b9-%d1%80%d0%be%d0%bb%d0%b8)
      - [Автоматизированное тестирование в travic-ci внешней роли db средствами molecule в gce](#%d0%90%d0%b2%d1%82%d0%be%d0%bc%d0%b0%d1%82%d0%b8%d0%b7%d0%b8%d1%80%d0%be%d0%b2%d0%b0%d0%bd%d0%bd%d0%be%d0%b5-%d1%82%d0%b5%d1%81%d1%82%d0%b8%d1%80%d0%be%d0%b2%d0%b0%d0%bd%d0%b8%d0%b5-%d0%b2-travic-ci-%d0%b2%d0%bd%d0%b5%d1%88%d0%bd%d0%b5%d0%b9-%d1%80%d0%be%d0%bb%d0%b8-db-%d1%81%d1%80%d0%b5%d0%b4%d1%81%d1%82%d0%b2%d0%b0%d0%bc%d0%b8-molecule-%d0%b2-gce)
      - [Прочие изменения](#%d0%9f%d1%80%d0%be%d1%87%d0%b8%d0%b5-%d0%b8%d0%b7%d0%bc%d0%b5%d0%bd%d0%b5%d0%bd%d0%b8%d1%8f)
- [Makefile](#makefile)
  - [Переменные](#%d0%9f%d0%b5%d1%80%d0%b5%d0%bc%d0%b5%d0%bd%d0%bd%d1%8b%d0%b5)
    - [Общие](#%d0%9e%d0%b1%d1%89%d0%b8%d0%b5)
    - [Packer](#packer)
    - [Terraform](#terraform)
    - [Tflint](#tflint)
    - [Ansible](#ansible)
  - [Цели](#%d0%a6%d0%b5%d0%bb%d0%b8)
    - [Устанока зависимостей](#%d0%a3%d1%81%d1%82%d0%b0%d0%bd%d0%be%d0%ba%d0%b0-%d0%b7%d0%b0%d0%b2%d0%b8%d1%81%d0%b8%d0%bc%d0%be%d1%81%d1%82%d0%b5%d0%b9)
    - [Packer](#packer-1)
    - [Terraform](#terraform-1)
    - [Ansible](#ansible-1)
    - [Vagrant](#vagrant)
    - [Aliases](#aliases)

# Домашние задания

## HomeWork 2: GitChatOps

* Создан шаблон PR
* Создана интеграция с TravisCI
```bash
 travis encrypt "devops-team-otus:<ваш_токен>#<имя_вашего_канала>" --add notifications.slack.rooms --com
```
* Создана интеграция с чатом для репозитория
* Создана интеграция с чатом для TravisCI
* Отработаны навыки работы с GIT

## HomeWork 3: Знакомство с облачной инфраструктурой. Google Cloud Platform

* Создана УЗ в GCP
* Созданы 2 ВМ: bastionhost с внешним IP и someinternalhost тосько с внутренним ip
* Настроено сквозное подключение по SSH к хосту someinternalhost посредством выполнения команды
`ssh someinternalhost` для чего:
  * при создании ВМ сгенерирован ssh-ключ `appuser`
  * ключ appuser добавлен в ssh-агент
  * в файл `~/.ssh/config` добавлены строки
    ```
    Host bastionhost
        IdentityFile ~/.ssh/appuser
        User appuser
        HostName 34.89.159.155
    Host someinternalhost
        IdentityFile ~/.ssh/appuser
        User appuser
        HostName 10.156.0.4
        ProxyJump bastionhost
    ```
  В результате, при выполнении команды `ssh someinternalhost`, происходит следующее:
  * Устанавливается соединение с `bastionhost` посредством подключения к `appuser@34.89.159.155` с использованием ключа `~/.ssh/appuser`
  * С хоста `bastionhost` устанавливается перенаправление TCP на `someinternalhost` посредством подключения к `appuser@10.156.0.4` с использованием ключа `~/.ssh/appuser`, это происходит даже если не добавлять ключ `~/.ssh/appuser` в ssh-agent
  * Аналогом директивы ProxyJump может быть опция `-J <jump host>` команды `ssh`, например
    ```shell
    ssh-add -L ~/.ssh/appuser
    ssh -i ~/.ssh/appuser -J appuser@34.89.159.155 appuser@10.156.0.4
    ```
    В случае такого способа, ssh-ключь должен быть добавлен в ssh-агент, иначе возникает ошибка
    ```
    appuser@34.89.159.155: Permission denied (publickey).
    ssh_exchange_identification: Connection closed by remote host
    ```
* Установлен и настроен vpn-сервер [pritunl](https://pritunl.com)
  ```
  bastion_IP = 34.89.159.155
  someinternalhost_IP = 10.156.0.4
  ```
  * Создана организация
  * Создан пользователь
  * Создан сервер
  * Добавлен маршрут ко внутренней сети
  * Сервер прикреплён к организации
* Административный интерфейс доступен так же по адресу https://34-89-159-155.sslip.io через sslip.io
* Создано доменное имя bastion.vscoder.ru, разрешаемое в ip 34.89.159.155
* При подключении к https://bastion.vscoder.ru используется сертификат от Let's Encrypt

## HomeWork 4: Деплой тестового приложения

### Основное задание

* Установлен и настроен [gcloud](https://cloud.google.com/sdk/gcloud/) для работы с нашим аккаунтом
* Создан хост с помощью gcloud
  ```
  gcloud compute instances create reddit-app\
    --boot-disk-size=10GB \
    --image-family ubuntu-1604-lts \
    --image-project=ubuntu-os-cloud \
    --machine-type=g1-small \
    --tags puma-server \
    --restart-on-failure
  ```
* Установлен ruby
* Установлен MongoDB 3.2
* Задеплоено тестовое приложение
  ```
  testapp_IP = 35.233.91.245
  testapp_port = 9292
  ```

### Самостоятельная работа

Создано 3 скрипта, реализующие все необходимые действия для развёртывания приложения на вновь созданном хосте:
* `install_ruby.sh` - для установки ruby
* `install_mongodb.sh` - для установки MongoDB
* `deploy.sh` - дял деплоя приложения

### Дополнительное задание 1

Создан скрипт `init.sh`, который
* На основе install_ruby.sh, install_mongodb.sh и deploy.sh, один общий скрипт `startup.sh`
  ```
  cat install_ruby.sh install_mongodb.sh deploy.sh > startup.sh
  ```
* Выполняет команду gcloud, которая создаёт инстанс ВМ и инициализирует его, запуская `startup.sh`, если инстанс с таким именем ещё не был создан
  ```
  gcloud compute instances create reddit-app\
    --boot-disk-size=10GB \
    --image-family ubuntu-1604-lts \
    --image-project=ubuntu-os-cloud \
    --machine-type=g1-small \
    --tags puma-server \
    --restart-on-failure \
    --metadata-from-file startup-script=startup.sh
  ```

### Дополнительное задание 2

Скрипт `init.sh` изменён таким образом, чтобы:
* Вместо использования локального startup-скрипта при инициальзации ВМ, загружает `startup.sh` в bucket на File Storage и создаёт ВМ посредством команды
  ```
  gcloud compute instances create reddit-app\
    --boot-disk-size=10GB \
    --image-family ubuntu-1604-lts \
    --image-project=ubuntu-os-cloud \
    --machine-type=g1-small \
    --tags "puma-server" \
    --restart-on-failure \
    --metadata startup-script-url=gs://vscoder-otus-hw4/startup.sh
  ```
* Создаёт правило фаервола _default-puma-server_, которое разрешает доступ на инстансы с тэгом _puma-server_ на tcp port 9292
  ```
  gcloud compute firewall-rules create default-puma-server \
  --allow=tcp:9292 \
  --target-tags="puma-server"
  ```

### Прочее

* Инициализация переменных перенесена в файл `.env`, который, в свою очередь, импортируется в `init.sh` командой
  ```
  source .env
  ```
* Добавлен скрипт `clean.sh`, который удаляет созданные объекты GCP
* При повторном запуске `init.sh`, ресурсы заново не создаются. Только выводится информация о созданном инстансе. Например:
  ```
  *** Check instance 'reddit-app' exists
  VM external IP is 35.233.91.245
  *** Create firewall rule, if not exists
  Completed. Service will be accessible soon at http://35.233.91.245:9292
  ```

## HomeWork 5: Сборка образов VM при помощи Paker

### Основное задание

* Установлен [packer](https://www.packer.io/downloads.html)
* Выполнена авторизация `gcloud auth application-default login`
* Создан файл `packer/ubuntu16.json` с описанием базового образа _reddit-base_
* Из [cloud-testapp](https://github.com/Otus-DevOps-2019-08/vscoder_infra/tree/cloud-testapp) скопированы и адаптированы скрипты установки ruby и MongoDB
* Скрипты добавлены в секцию _provisioning_ описания образа
* Успешно собран образ командой `packer build ubuntu16.json`
* Для автоматизации создания образа создан скрипт `init_base.sh`
* На основе образа _reddit-base_ развёрнут экземпляр ВМ
* На ВМ развёрнут puma server с тестовым приложением

### Самостоятельные задания

* Параметризованы переменные
* Добавлен файл-пример с обязательными переменными `variables.json.example`
  Важно: если задать значение переменной _network_ отличное от **default**, необходимо предварительно создать соответствующую сеть. Необходимо так же задать значение параметру _subnetwork_
  >  Only required if the network has been created with custom subnetting. Note, the region of the subnetwork must match the region or zone in which the VM is launched. [link](https://www.packer.io/docs/builders/googlecompute.html#subnetwork)

* Создана сеть `testnetwork`
* Для сети создано **правило брендмауера**, разрешающее доступ к 22 порту (иначе packer не может подключиться к ВМ)

### Первое задание со *

* Создан шаблон `immutable.json` с описанием образа _reddit-full_, основаного на _reddit-base_ и содержащего в себе развёрнутое приложение
* Приложение разворачивается скриптом `deploy.sh`, в процессе развёртывания:
  * Склонирован github-репозиторий
  * Установлены зависимости
  * Обеспечен запуск сервера приложения посредством systemd unit-файла
    Содержимое `reddit-app.service` файла описано непосредственно в скрипте `deploy.sh`
  * Включена автозагрузка `reddit-app.service`
  * Проверена работоспособность `reddit-app.service`:
    * Старт
    * Рестарт
    * Статус
    * Стоп
* В случае успешного выполнения всех шагов скрипта, создаётся и заливается в GCP packer-образ _reddit-full_
* Для автоматизации описаных шагов создан скрипт `init_full.sh`

### Второе задание со *

Создан скрипт `config-scripts/create-reddit-vm.sh`, который:
* С помощью утилиты `gcloud` создаёт ВМ _reddit-full_, если такой не существует (иначе пропускает этот шаг)
  ВМ создаётся с тегом _puma-server_
* Сообщает пользователю белый IP созданной или существующей ВМ
* Создаёт правило фаервола _default-puma-server_ (если не существует), которое разрешает трафик на tcp-порт 9292 всех ВМ с тегом _puma-server_
* Сообщает пользователю URL для подключения к запущенному приложению

Замечание: указанный скрипт проверяет существования экземпляра ВМ и правила фаервола только по имени. В случае если экземпляр ВМ или правило фаервола с соответствующим именем уже существует, но отличается по свойствам, оно пересоздано **не будет**! Необходимо вручную удалить соответствующий объект чтобы скрипт создал его заново с нужными свойствами.

## HomeWork 6: Практика IaC с использованием Terraform

### Основное задание

* Установлен terraform
* В `.gitignore` добавлены временные и приватные файлы terraform-проекта
* Создан файл `main.tf`, в который добавлены секции
  * _terraform_ требованиями к версии `terraform`
  * _provided "google"_ со специфичными для GCP параметрами
* Выполнена авторизация terraform в google
  ```
  gcloud auth application-default login
  ```
* Проект проинициализирован командой `terraform init`, в процессе чего загружены необходимые для работы с GCP модули
* В `main.tf` добавлено базловое описание инстанса ВМ
  * имя
  * тип
  * зона
  * семейство образов загрузочного диска (будет браться последняя версия)
  * сетевой интерфейс
* Создан экземпляр ВМ
  ```
  terraform plan
  terraform apply
  ```
  Поле этого создаётся файл `terraform.tfstate` с описанием текущей инфраструктуры
  **Важно:** Если базовый образ был обновлён после создания инстанса ВМ, это никак не повлияет на уже созданную ВМ. Для использования нового базового образа, инстанс ВМ нужно пересоздать посредством команды `terraform taint google_compute_instance.<resource name>`
* Добавлены метаданные, оисывающие публичный ключ, который необходимо загрузить на созданный инстанс
  ```
  resource ... {
  ...
    metadata = {
      ssh-keys = "user"${file("path_to_key.pub")}"
    }
  ...
  }
  ```
  **Примечание:** Работает так же для уже созданной ВМ. После применения изменений, к инстансу удалось подключиться пл ssh
* Создан файл `outputs.tf` со списком переменных, показываемых после применения изменений. В этот файл добавлен внешний адрес созданного инстанса
  ```
  output "app_external_ip" {
    value = google_compute_instance.<resource_name>.network_interface[0].access_config[0].nat_ip
  }
  ```
* В файл `main.tf` добавлен ресурс _google_compute_firewall_ с описанием правила фаервола, разрешающего доступ к порту сервера приложения. Соответствующий тег добавлен к экземпляру ВМ
* В проект добавлены файлы `files/puma.service` и `files/deploy.sh`, необходимые для провиженинга создаваемого инстанса
* В файл `main.tf` в ресурс _google_compute_instance_ добавлены 2 провиженера:
  * тип _file_ для копирования systemd unit- файла на инстанс
    ```
    provisioner "file" {
      source      = "files/puma.service"
      destination = "/tmp/puma.service"
    }
    ```
  * тип _remote-exec_ для запуска на инстансе скрипта `files/deploy.sh`
    ```
    provisioner "remote-exec" {
      script = "files/deploy.sh"
    }
    ```
  * Описана секция _connection_ с описанием способа подключения провиженеров к инстансу ВМ
* С целью выполнения провиженеров, пересоздане экземпляра ВМ форсировано командой `terraform taint google_compute_instance.<resource name>`
* Посредством использования input-переменных параметризованы следующие параметры:
  * _project_ имя проекта
  * _region_ регион
  * _public_key_path_ путь к публичному ssh-ключу, загружаемому на инстанс ВМ
  * _disk_image_ имя базового образа для загрузочного диска
* Обязательные параметры определены в файле `terraform.tfvars`, который игнорируется git-ом

### Самостоятельные задания

* Определена обязательная input-переменная _private_key_path_, значением которой является путь к закрытому ssh-ключу, использующемуся при подключени провиинеров
* Определена input-переменная _zone_, задающая зону, в которой должен создаваться экземпляр ВМ
* Все `*.tf` файлы отформатированы командой `terraform fmt`
* Создан файл ` terraform.tfvars.example` с примерами обязательных переменных

### Задания со *

* Добавлен публичный ssh-ключ, общий для всего проекта
  ```
  resource "google_compute_project_metadata_item" "sshkey-appuser1" {
    key = "ssh-keys"
    value = "appuser1:${file(var.public_key_path)}"
  }
  ```
  После применения, на ранее созданной ВМ автоматически был создан пользователь _appuser1_ с добавленным к нему указанным ключом. Попытка подключения по ssh под именм данного пользователя прошла успешно.
* Добавлены публичные ключи для пользователей _appuser2_ и _appuser3_
  ```
  resource "google_compute_project_metadata_item" "ssh-keys1" {
    key = "ssh-keys"
    value = "appuser1:${file(var.public_key_path)}"
  }
  resource "google_compute_project_metadata_item" "ssh-keys2" {
    key = "ssh-keys"
    value = "appuser2:${file(var.public_key_path)}"
  }
  resource "google_compute_project_metadata_item" "ssh-keys3" {
    key = "ssh-keys"
    value = "appuser3:${file(var.public_key_path)}"
  }
  ```
  После применения, в метаданные проекта был добавлен только пользователь _appuser1_, а так же определённый для инстанса _appuser_. Подключение под обоими прошло успешно.
* Дополнительные ключи добавлены в один ресурс
  ```
  resource "google_compute_project_metadata_item" "ssh-keys" {
  key = "ssh-keys"
  value = <<EOF
    appuser1:${file(var.public_key_path)}
    appuser2:${file(var.public_key_path)}
    appuser3:${file(var.public_key_path)}
  EOF
  }
  ```
  После применения ключи в метаданные проекта добавлены, но на развёрнутый инстанс пользователи не приехали. В веб-интерфейсе в метаданных проекта появилось так же несколько _пустых_ ssh-ключей, с незаполненными значениями.
* Рабочим оказалось следующее решение:
  * `main.tf`
  ```
  resource "google_compute_project_metadata_item" "ssh-keys" {
    key = "ssh-keys"
    value = join("\n", var.ssh_keys)
  }
  ```
  * `variables.tf`
  ```
  variable ssh_keys {
    type    = list(string)
  }
  ```
  * `terraform.tfvars`
  ```
  ssh_keys = [
    "appuser:ssh-rsa <key_value_here> appuser",
    "appuser1:ssh-rsa <key_value_here> appuser",
    "appuser2:ssh-rsa <key_value_here> appuser",
    "appuser3:ssh-rsa <key_value_here> appuser"
  ]
  ```
  На инстансе были созданы все 4 пользователя
  **Примечание:** Экспериментальным путём установлено, что использование параметра метаданных `block-project-ssh-keys = false` необязательно
  **Примечание:** Использовать функцию `file()` при задании значений переменных в файле `terraform.tfvars` не удалось, так как не поддерживается. TODO: Выяснить как это реализовать
* Выполнена попытка добавить ключ пользователя _appuser_ с комментарием _appuswer_web_. В результате gcp выдал ошибку
  ```
  Supplied fingerprint does not match current metadata fingerprint.
  ```
  и дальнейшие попытки изменить состав ключей были неудачными
* В веб-интерфейса заново открыт список ключей, далее:
  * Сгенерирован новый ssh-ключ _appuser_web_
  ```
  ssh-keygen -t rsa -f ~/.ssh/appuser_web -C appuser_web -P ""
  ```
  * Сгенерированный ключ добавлен в метаданные проекта через веб-нитерфейс -- ключ успешно был добавлен, но войти под пользователем _appuser_web_ **не удалось** -- ошибка авторизации
  * Выполнено применение инфраструктуры `terraform apply` -- terraform созданный вручную ключ удалил

### Задания с **

При разработке использовались следующие ресурсы:
* https://cloud.google.com/load-balancing/docs/https/

Что было сделано:
* Создан файл `lb.tf`, в котором описаны следующие сущности:
  * google_compute_instance_group со списком инстансов ВМ с запущенным приложением (пока 1 экземпляр)
  * google_compute_health_check для проверки доступности приложения на экземпляре ВМ
  * google_compute_backend_service со ссылкой на группы экземпляров ВМ (в данном случае на 1 группу), а так же со ссылкой на google_compute_health_check
  * google_compute_url_map с описанием запросу к какому url на какой backend_service отправлять (в нашем случае все запросы ко всем url отправляются на 1 сервис)
  * google_compute_target_http_proxy для проксирования http/https соединений к url_map
  * google_compute_global_forwarding_rule для перенаправления ip4/ip6 трафика (для каждого типа трафика должно быть своё правило) на target_http_proxy (в нашем случае только ip4)
  * так же была добавлена output-переменная, выводящая ip балансировщика
* Изменение количества инстансов было реализовано посредством добавления имени нового инстанса в множество _instances_ в файл `terraform.tfvars`
* Output-переменная _app_external_ip_ теперь отображает список ip-адресов всех инстансов
* Добавлен второй инстанс ВМ с приложением. Решены возникшие в процессе настройки проблемы.
  **Важно:** google compute backend service очень долго стартует, в результате чего приложение через балансировщик становится доступным спустя продолжительное время (возможно более 10 минут)
* Выполнена остановка приложения на одном из инстансов. Интерфейс приложения остался доступен через балансировщик как и прежде.
* Код изменён таким образом, чтобы использоать переменную _instance_count_, указывающую количество необходимых инстансов, вместо _instances_, содержащей множество имён необходимых инстансов
  * _variables.tf_
    ```
    variable instance_count {
      type    = number
      default = 1
    }
    ```
  * _main.tf_
    ```
    resource "google_compute_instance" "app" {
      name         = "reddit-app${count.index}"
      count        = var.instance_count
      ...
    }
    ```
  * _outputs.tf_
    ```
    output "app_external_ip" {
      value = google_compute_instance.app[*].network_interface[0].access_config[0].nat_ip
    }
    ```
  * _lb.tf_
    ```
    resource "google_compute_instance_group" "app_instance_group" {
      instances = google_compute_instance.app[*].self_link
      ...
    ```
* Протестирована отказоустойчивость

## HomeWork 7: Принципы организации инфраструктурного кода и работа над инфраструктурой в команде на примере Terraform

### Основное задание

* Файл `lb.tf` из предыдущего задания с ** перемещён в поддиректорию `terraform/files/`
* В `main.tf` описано правило фаервола `firewall_ssh`
  При применении возникла ошибка
  ```
  Error: Error creating Firewall: googleapi: Error 409: The resource 'projects/infra-253214/global/firewalls/default-allow-ssh' already exists, alreadyExists
  ```
  так как правило с таким именем уже присутствует в проекте
* Выполнен импорт правила из GCP в terraform state
  ```
  terraform import google_compute_firewall.firewall_ssh default-allow-ssh
  ```
* К ресурсу добавлено описание правила. Изменения применены `terraform apply`

* В `main.tf` определён ресурс `google_compute_address.app_ip reddit-app-ip`
* Инфраструктура пересоздана
  ```
  terraform destroy
  terraform apply
  ```
* Добавлена ссылка google_compute_instance.app network_interface access_config nat_ip на созданный статический ip

* Создан файл `packer/db.json`, описывающий packer-образ `reddit-db-base` для БД (mongodb)
* Создан файл `packer/app.json`, описывающий packer-образ `reddit-app-base` для app (ruby)
* Создан скрипт `packer/build_image.sh` для создания образов из json-файлов
* Запечены образы `reddit-db-base` и `reddit-app-base`
  ```
  ./build_image.sh db.json
  ./build_image.sh app.json
  ```

* Добавлен файл `terraform/app.tf` с описанием создания инстанса `reddit-app`, а так же:
  * статисеского адреса
  * правила фаервола
* Добавлен файл `terraform/db.tf` с описанием создания инстанса `reddit-db`, а так же:
  * правила фаервола
* Из `terraform/main.tf` убрано описание
  * инстанса `reddit-app`
  * правила фаервола для доступа к `reddit-app`
  * статического ip-адреса
* В `terraform/variables.tf` добавлены пеерменные базовых образов диска для app и db
  * app_disk_image
  * db_disk_image
* Правило фаервола для доступа к ssh вынесено из `terraform/main.tf` в `terraform/vpc.tf`
* Метаданные проекта вынесены из `terraform/main.tf` в `terraform/metadata.tf`
* Требования к версии terraform вынесены из `terraform/main.tf` в `terraform/metadata.tf`

* В директории `terraform/` создана поддиректория `modules/` для описания локальных модулей
* Описание инстанса `reddit-app` перенесено в модуль `modules/app/`, а так же
  * описание статического ip
  * описание правила фаервола
  * входящие переменные `public_key_path`, `zone`, `app_disk_image`
  * выходящая переменная `app_external_ip` (впоследствии будет получена в `outputs.tf` основного модуля)
* Описание инстанса `reddit-db` перенесено в модуль `modules/db/`, а так же
  * описание правила фаервола
  * входящие переменные `public_key_path`, `zone`, `db_disk_image`
* Созданные модули загружены в проект
  ```
  terraform get
  ```
* Правило фаервола для ssh перенесено из `vpc.tf` в отдельный модуль `modules/vpc/`, а так же:
  * входящяя переменная `zone`
* Созданные модули загружены в проект
  ```
  terraform get
  ```
* Инфраструктура создана `terraform apply`
* Успешно выполнено подключение по ssh к созданному инстансу
* Параметризована переменная `source_ranges` модуля `vpc`
* Протестирована работа переменной `source_ranges`
  * При задании своего белого ip подключение по ssh к созданному инстансу выполняется успешно
  * При задании любого другого белого ip, подключение не удалось
    *ЗАМЕЧАНИЕ:* Фактичетски изменение `source_ranges` применяется спустя несколько десятков секунд после завершения выполнения команды `terraform apply`

* Конфигурация разнесена по 2-м окружениям
  * *stage* - доступ к ssh открыт со всех ip
  * *prod* - доступ к ssh открыт только с моих ip
* Из корня terraform-проекта удалены файлы, скопированные в каждое из окружений
  * `terraform/main.tf`
  * `terraform/outputs.tf`
  * `terraform/variables.tf`
  * `terraform/terraform.tfvars`
* Проверена правильность настроке инфраструктуры каждого из окружений посредством `terraform apply`
* Для модулей параметризовано имя окружения (stage/prod)
* Для каждого окружения создаётся отдельная сеть с именем `${var.network_name}-${var.environment}`
* Для модуля app параметризовано создание ресурса `google_compute_address`, а так же назначение его инстансу.
  Создание ресурса только если `var.use_static_ip` истина
  ```
  resource "google_compute_address" "app_ip" {
    name = "reddit-app-ip-${var.environment}"
    count = var.use_static_ip ? 1 : 0
  }
  ```
  Назначение статического адреса только если `var.use_static_ip` истина
  ```
  network_interface {
    network = "${var.network_name}-${var.environment}"
    access_config {
      nat_ip = var.use_static_ip ? google_compute_address.app_ip[0].address : null
    }
  }
  ```
* Добавлен файл `storage-bucket.tf`, содержащий модуль `SweetOps/storage-bucket/google`
* Для загрузки недостающих модулей выполнен `terraform init`
* Для функционирования в секцию `module` понадобилось добавить/изменить передаваемые параметры
  ```
  name     = "storage-bucket-test-${var.project}"
  location = var.region
  ```
* Проверена работоспособность `terraform apply`

### Задания со * Хранение state в gcs

**ВАЖНО:** Перед изменением `backend.tf` не забывать удалять текущую инфраструктуру `terraform destroy`

**Примечание:** дял корректной работы с `backend` понадобилось убрать подстановку переменной в имя `storage-bucket`, так как *the backend configuration does not support variables or expressions of any sort*. Работу с переменными в бэкэндах, а так же поддерживать инфраструктурный код *DRY and maintenable* позволяет [terragrunt](https://github.com/gruntwork-io/terragrunt)

* Создан `stage/backend.tf` с описанием remote backend для хранения состояния
  ```
  terraform {
    backend "gcs" {
      bucket = "vscoder-otus-tf-state"
      prefix = "terraform/state"
    }
  }
  ```
* Файлы `*.tfstate*` и `.terraform` вынесены из репозитория во внешнюю директорию
* Выполнена инициализация `terraform init`
* stage-инфраструктура развёрнута `terraform apply`.
  Как и ожидалось, файлы состояния в директории не появились:
  ```
  .
  ├── backend.tf
  ├── main.tf
  ├── outputs.tf
  ├── terraform.tfvars
  ├── terraform.tfvars.example
  └── variables.tf

  0 directories, 6 files
  ```
* Файл `stage/backend.tf` скопирован в `prod/backend.tf` без изменений
* При выполнении `terraform plan` - все ресурсы запланированы к пересозданию. Такое поведение не устраивает.
  ```
  Plan: 7 to add, 0 to change, 6 to destroy.
  ```
* В обоих окружениях в `backend.tf` изменён `prefix`
  Было: `prefix = "terraform/state"`
  Стало: `prefix = "terraform/state/stage"` и `prefix = "terraform/state/prod"` соответственно
* Применение инфраструктуры (`terraform apply`) для каждого из окружений прошло успешно. Одновременно.
* `terraform show` для каждого из окружений выдаёт свой набор объектов
* При попытке применить изменения (`terraform apply`) одновременно (из разных терминалов) для одного окружения, во втором терминале terraform выдал ошибку:
  ```
  Error: Error locking state: Error acquiring the state lock: writing "gs://vscoder-otus-tf-state/terraform/state/prod/default.tflock" failed: googleapi: Error 412: Precondition Failed, conditionNotMet
  ```
  что говорит о корректной работе блокировок

### Задание с ** Провиженинг приложения с использованием пременных окружения

* В модуль `db` добавлена output-переменная `db_internal_ip` для передачи в модуль `app`
  ```
  output "db_internal_ip" {
    value = google_compute_instance.db.network_interface[0].network_ip
  }
  ```
* В окружении `stage` данная переменная передаётся модулю `app` как часть переменной `database_url`
  ```
  database_url    = "${module.db.db_internal_ip}:27017"
  ```
* В модуле `app`
  * создана input variable `database_url` для передачи провиженеру
    ```
    variable database_url {
      description = "MongoDB url. Ex: 127.0.0.1:27017"
    }
    ```
  * в `google_compute_instance` добавлены провиженеры
    * заполняющий на основе переменной `var.database_url` файл `puma.env`
      ```
      provisioner "file" {
        content      = "DATABASE_URL=${var.database_url}"
        destination = "/tmp/puma.env"
      }
      ```
    * передающий на инстанс шаблон systemd-юнита для запуска puma server
      ```
      provisioner "file" {
        source      = "${path.module}/files/puma.service.tmpl"
        destination = "/tmp/puma.service.tmpl"
      }
      ```
    * выполняющий на инстансе скрипт `deploy.sh`
      ```
      provisioner "remote-exec" {
        script = "${path.module}/files/deploy.sh"
      }
      ```
  * В шаблоне systemd-юнита `puma.service.tmpl`:
    * параметризован путь к директории с приложением
    * параметризован пользователь от имени которого запускается приложение
    * Добавлен параметр `EnvironmentFile` для передачи переменных из файла `puma.env` в качестве переменных окружения запускаемому приложению
      ```
      [Service]
      EnvironmentFile=${APP_DIR}/puma.env
      ...
      ```
  * В файле `deploy.sh` выполняются следующие действия:
    * экспортируется переменная `$APP_DIR` для корректной подстановки в шаблон systemd-юнита
    * из репозитория устанавливается приложение в `$APP_DIR`
    * файл с переменными окружения `puma.env` перемещается из временной директории в `$APP_DIR`
    * в systemd добавляется сервис `puma.service` из шаблона `/tmp/puma.service.tmpl`
      ```
      cat /tmp/puma.service.tmpl | envsubst | sudo tee /etc/systemd/system/puma.service
      ```
    * `puma.service` запускается и добавляется в автозагрузку
  * Помимо перечисленного, в stage-окружение добавлены дополнительные output variables
* **НО** при запуске приложения, оно не смогло подключиться к БД по причине того, что MongoDB по умолчанию запускается на адресе `127.0.0.1`

* Запуск mongod сервиса на `0.0.0.0` исправлен добавлением в модуль `db` провиженера, заменяющено `bindIp: 127.0.0.1` на `bindIp: 0.0.0.0` в конфигурационном файле `mongod.conf` и перезапускающего сервис
  ```
  provisioner "remote-exec" {
    inline = [
      "sudo sed -i.bak 's/bindIp: 127.0.0.1/bindIp: 0.0.0.0/' /etc/mongod.conf",
      "sudo systemctl restart mongod.service"
    ]
  }
  ```
* Приложение **работает** на http://<app_external_ip>:9292

* Изменения конфигурационного файла MongoDB реализовано **на этапе сборки базового образа** средствами packer, так как это более правильный способ
* Провиженер из модуля `db` ресурса `google_compute_instance` **убран** за ненадобностью

* Скорректирован порядок создания модулей за счёт использования output переменной с именем созданной сети в модуле `vpc`, как входящей переменной с именем сети для модулей `app` и `db`

* `prod` окружение обновлено до того же состояния, что и `stage`

## HomeWork 8: Управление конфигурацией. Основные DevOps инструменты. Знакомство с Ansible

### Основное задание

* В директории `ansible/` создано виртуальное окружение python, в которое установлен Ansible
  ```
  cd ansible/
  python3 -m venv .venv
  source .venv/bin/activate
  pip install -r requirements.txt
  ```
* Проверена установка ansible
  ```
  # ansible --version
  ansible 2.8.5
    config file = /etc/ansible/ansible.cfg
    configured module search path = ['/home/vscoder/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
    ansible python module location = /mnt/calculate/home/vscoder/projects/otus/devops201908/vscoder_infra/ansible/.venv/lib/python3.6/site-packages/ansible
    executable location = /mnt/calculate/home/vscoder/projects/otus/devops201908/vscoder_infra/ansible/.venv/bin/ansible
    python version = 3.6.8 (default, Oct  7 2019, 12:59:55) [GCC 8.3.0]
  ```
* Развёрнута stage-инфраструктура Terraform
  ```
  cd ../terraform/stage
  terraform apply
  ```
* Создан inventory-файл `ansible/inventory` с указанием параметров подключения к поднятому terraform хосту reddit-app
* Проверена возможность управления
  ```
  ansible appserver -i ./inventory -m ping
  ```
* В Terraform-модуль db, а так же в stage и prod окружения добавлена выходная переменная db_external_ip
* В ansible inventory добавлен хост dbserver. Проверена доступность
  ```
  ansible dbserver -i ./inventory -m ping
  ```
* Общие параметры подключения перенесены из inventory в конфиг `ansible/ansible.cfg`
  ```
  [defaults]
  inventory =  # путь к inventory-файлу
  remote_user =  # ssh пользователь
  private_key_file =  # путь к закрытому ssh-ключу
  host_key_checking =  # проверка ssh host fingerprint удалённых хостов
  retry_files_enabled =  # создание .retry файлов в случае неудачного завершения плейбука
  ```
* Проверен аптайм инстанса dbserver
  ```
  ansible dbserver -m command -a uptime
  ```
* Хосты в inventory разделены по группам
  ```
  [app]
  appserver ansible_host=<app_external_ip>
  [db]
  dbserver ansible_host=<db_external_ip>

  ```
* Создан аналогичный inventory в yaml-формате `ansible/inventory.yml`. Ansible настроен на использование нового инвентаря
  ```
  ---
  all:                    # группа со всеми хостами
    children:             # дочерние группы
      app:                # группа app
        hosts:            # хосты в группе app
          appserver:      # хост appserver
            ansible_host: <app_external_ip>  # переменная хоста
      db:                 # группа db
        hosts:            # группа db
          dbserver:       # хост dbserver
            ansible_host: <db_external_ip> # переменная хоста
  ```
* Проверены различия в работе модулй `command` и `shell`
  * command:
    ```
    # ansible app -m command -a 'ruby -v'
    appserver | CHANGED | rc=0 >>
    ruby 2.3.1p112 (2016-04-26) [x86_64-linux-gnu]
    ```
    ```
    # ansible app -m command -a 'ruby -v; bundler -v'
    appserver | FAILED | rc=1 >>
    ruby: invalid option -;  (-h will show valid options) (RuntimeError)non-zero return code
    ```
  * shell:
    ```
    # ansible app -m shell -a 'ruby -v; bundler -v'
    appserver | CHANGED | rc=0 >>
    ruby 2.3.1p112 (2016-04-26) [x86_64-linux-gnu]
    Bundler version 1.11.2
    ```
* Проверен статус mongod модулем `command` (*bashsible anipattern*)
  ```
  # ansible db -m command -a 'systemctl status mongod'
  dbserver | CHANGED | rc=0 >>
  ...
  ```
* Проверен статус mongod модулями `systemd` и `service` (*true way*)
  systemd
  ```
  # ansible db -m systemd -a name=mongod
  dbserver | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python"
    },
    "changed": false,
    "name": "mongod",
    "status": {
  ...
  ```
  service
  ```
  # ansible db -m service -a name=mongod
  dbserver | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python"
    },
    "changed": false,
    "name": "mongod",
    "status": {
  ...
  ```
* Протестировано повторное выполнение модулей `git` и `command`. `git` идемпотентен, `command` - нет. Модуль `git` отработал успешно несколько раз, сообщив об отсуттствии изменений. Модуль `command` выдал ошибку:
  ```
  # ansible app -m command -a 'git clone https://github.com/express42/reddit.git /home/appuser/reddit'
  appserver | FAILED | rc=128 >>
  fatal: destination path '/home/appuser/reddit' already exists and is not an empty directory.non-zero return code
  ```
* Создан простой плейбук [clone.yml](ansible/clone.yml), выполняющий клонирование репозитория с приложением
  ```
  - name: Clone
    hosts: app
    tasks:
      - name: Clone repo
        git:
          repo: https://github.com/express42/reddit.git
          dest: /home/appuser/reddit
  ```
* Протестировано выполнение плейбука при наличии склонированного репозитория и после его удаления. Поведение ожидаемое:
  * при наличии репозитория изменеий не произведено
  * после удаления - заново клонируется репозиторий

### Задание со \*: Работа с динамическим inventory

* Создан файл [inventory.json](ansible/inventory.json) содержащий json в формате динамического инвентаря
  ```
  ansible-inventory --list > inventory.json
  ```
* Создан python-скрипт [json2inv.py](ansible/json2inv.py) который, при запуске с параметром `--list`, возвращает json из файла `inventory.json`, предварительно проверив его на корректность
  ```
  usage: json2inv.py [-h] [--json-file JSON_FILE] [-l] [--host HOST] [-d]

  Read json file and print them content to stdout. Author: Aleksey Koloskov
  <vsyscoder@yandex.ru>

  optional arguments:
    -h, --help            show this help message and exit
    --json-file JSON_FILE
                          path to dynamic json-inventory file (default:
                          ./inventory.json)
    -l, --list            print json content to stdout (default: False)
    --host HOST           print single host variables (default: None)
    -d, --debug           print debug messages (default: False)
  ```
* В [ansible.cfg](ansible/ansible.cfg) прописан inventory-скрипт
  ```
  inventory = json2inv.py
  ```
* Протестирована работоспособность:
  ```
  # ansible -m ping all
  appserver | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python"
    },
    "changed": false,
    "ping": "pong"
  }
  dbserver | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python"
    },
    "changed": false,
    "ping": "pong"
  }
  ```
* Просто и понятно про статический inventory в формате json удалось найти здесь: https://stackoverflow.com/a/57768613/3488348
  * Статический json-inventory имеет ту же структуру, что и inventory в формате yaml (протестировано `ansible -i static-inventory.json -m ping all`)
  * Динамическй json-inventory -- это **обязательно** результат выполнения скрипта, имеющий несколько другую структуру. Подробнее можно узнать по ссылке: https://docs.ansible.com/ansible/latest/dev_guide/developing_inventory.html
* Исправлена ошибка, препятствующая запуску inventory-скрипта на python версии младше 3.6

## HomeWork 9: Деплой и управление конфигурацией с Ansible

### Основное задание

* Закомментирован провиженинг приложения средствами terraform
---
* Создан playbook [reddit_app.yml](ansible/reddit_app.yml) в котором с помощью модуля `template` генерируется конфиг для сервиса mongod
* Создан шаблон конфига сервиса mongod [mongod.conf.j2](ansible/templates/mongod.conf.j2)
* Выполнена проверка применения плейбука командой
  ```
  ansible-playbook reddit_db.yml --diff --check --limit db
  ```
* В плейбук добавлен хэндлер, который перезапускает сервис `mongod` если конфиг изменился.
* К задаче добавлена секция `notify`, которая сообщает о необходимости запуска хендлера.
---
* Добавлен systemd unit-файл [puma.service](ansible/files/puma.service) для запуска приложения
* В плейбук добавлена задача для копирования unit-файла на хост, модуль `copy`
* Добавлена задача, включающая автозапуск сервиса, модуль `systemd`
* Добавлен хэндлер, перезапускабщий сервис  при изменении unit-файла
* Добавлен шаблон [db_config.j2](templates/db_config.j2), содержащий переменные окружения для запускаемого сервиса. В частности, переменную `DATABASE_URL`, получающую значение из ansible-переменной `db_host`
* Добавлена задача для копирования шаблона с переменными окружения на хост
* Вручную задано значение переменной `db_host`, содержащей внутренний адрес инстанса db
* Добавлена задача по получению приложения из git-репозитория, модуль `git`
* Добавлена задача по установке зависимостей, модуль `bundler`
---
* Добавлен плейбук [reddit_app2.yml](playbooks/reddit_app2.yml)
* В плейбук добавлен сценарий `Configure MongoDB` с тегом `db-tag` для настройки и запуска MongoDB
* В плейбук добавлен сценарий `Configure App` с тегом `app-tag` дня настройки и автозапуска приложения
* В плейбук добавлен сценарий `Deploy App` с тегом `deploy-tag` для деплоя приложения
---
* Плейбук [reddit_app.yml](ansible/reddit_app.yml) переименован в [reddit_app_one_play.yml](ansible/reddit_app_one_play.yml)
* Плейбук [reddit_app2.yml](playbooks/reddit_app2.yml) переименован в [reddit_app_multiple_plays.yml](ansible/reddit_app_multiple_plays.yml)
* Создан плейбук [db.yml](ansible/db.yml) в который добавлен сценарий `Configure MongoDB` по развёртыванию MongoDB. Из сценария удалён тег
* Создан плейбук [app.yml](ansible/app.yml) в который добавлен сценарий `Configure App` по настройке приложения. Из сценария удалён тег
* Создан плейбук [deploy.yml](ansible/deploy.yml) в который добавлен сценарий `Deploy App` по настройке приложения. Из сценария удалён тег
* Добавлен плейбук [site.yml](ansible/site.yml), который, для настиройки всей инфраструктуры, поочерёдно запускает
  * [db.yml](ansible/db.yml)
  * [app.yml](ansible/app.yml)
  * [deploy.yml](ansible/deploy.yml)
* Проверена работоспособность вышеописанной конфигурации
  ```
  ansible-playbook --diff site.yml --check
  ansible-playbook --diff site.yml
  ```

### Задание со \*: Динамический inventory

#### Исследование

* Для использования динамического инвентаря google cloud platform, [официальная документации ansible](https://docs.ansible.com/ansible/latest/scenario_guides/guide_gce.html) предлагает использовать inventory plugin [gcp_compute](https://docs.ansible.com/ansible/latest/plugins/inventory/gcp_compute.html). Преимущества dynamic inventory plugin над dynamic inventory script, описаны [здесь](https://docs.ansible.com/ansible/latest/dev_guide/developing_inventory.html)
  ```
  In previous versions you had to create a script or program that can output JSON in the correct format when invoked with the proper arguments. You can still use and write inventory scripts, as we ensured backwards compatibility via the script inventory plugin and there is no restriction on the programming language used. If you choose to write a script, however, you will need to implement some features yourself. i.e caching, configuration management, dynamic variable and group composition, etc. While with inventory plugins you can leverage the Ansible codebase to add these common features.
  ```
* Описание параметров плагина `gcp_compute` [https://github.com/ansible/ansible/blob/devel/lib/ansible/plugins/inventory/gcp_compute.py](https://github.com/ansible/ansible/blob/devel/lib/ansible/plugins/inventory/gcp_compute.py)
* Для разбиения инстансов по группам можно использовать несколько [способов](https://docs.ansible.com/ansible/latest/plugins/inventory.html#using-inventory-plugins).
  * Пример JSON-представления тегов:
  ```
  "tags": {
    "fingerprint": "NQyRUqL7UTU=",
    "items": [
      "reddit-db"
    ]
  }
  ```
  * Статическое задание групп в зависимости от значений тегов:
    ```
    groups:
      # add hosts to the group 'db' if any of the dictionary's keys or values is the word 'reddit-db'
      db: "'reddit-db' in (tags['items']|list)"
      # add hosts to the group 'app' if any of the dictionary's keys or values is the word 'reddit-app'
      app: "'reddit-app' in (tags['items']|list)"
    ```
    на выходе получим
    ```
    "app": {
      "hosts": [
        "reddit-app-stage"
      ]
    },
    "db": {
      "hosts": [
        "reddit-db-stage"
      ]
    }
    ```
  * Чтобы более правильно группировать инстансы, [официальная документация terraform](https://www.terraform.io/docs/extend/best-practices/naming.html) рекомендует следующую схему назначения тэгов:
    ```
    tags          = {
      Name        = "Application Server"
      Environment = "production"
    }
    ```
    TODO: протестировать
  * Так же можно использовать [gcp labels](https://www.terraform.io/docs/providers/google/r/compute_instance.html#labels) - (Optional) A map of key/value label pairs to assign to the instance.
    TODO: протестировать
  * Так же можно реализовать разбиение по группам средствами `keyed_groups`:
    [terraform/modules/app/main.tf](terraform/modules/app/main.tf)
    ```
    resource "google_compute_instance" "app" {
      ...
      tags         = ["reddit-app"]
      ...
    ```
    [terraform/modules/db/main.tf](terraform/modules/db/main.tf)
    ```
    resource "google_compute_instance" "db" {
      ...
      tags         = ["reddit-db"]
      ...
    ```
    [ansible/infra.gcp.yml](ansible/infra.gcp.yml)
    ```
    keyed_groups:
      # Create groups from GCE labels
      - prefix: "group"
        separator: "_"
        key: tags['items']
    ```
    на выходе получим группы
    ```
    "group_reddit_app": {
        "hosts": [
            "reddit-app-stage"
        ]
    },
    "group_reddit_db": {
        "hosts": [
            "reddit-db-stage"
        ]
    }
    ```
* Для дебага значений переменных, можно в `tasks:` добавить следующую задачу
  ```
  - name: Debug
    debug:
      var: hostvars
    tags:
      - never
      - debug
  ```
  Чтобы вывести отладочную информацию, необходимо запустить `ansible-playbook` с `--tags debug`

#### Реализация

* Создан service account `ansible` с ролью `Compute Viewer` для просмотра инстансов.
* JSON credintials сохранены в директорию вне репозитория `~/.gce/`
* Создан файл [infra.gcp.yml](ansible/infra.gcp.yml) с настройками инвентаря
  ```
  plugin: gcp_compute
  projects:
    - infra-253214
  auth_kind: serviceaccount
  service_account_file: ~/.gce/infra-253214-ansible-1319bf6f5839.json
  hostnames:
    # List host by name instead of the default public ip
    - name
  compose:
    # Set an inventory parameter to use the Public IP address to connect to the host
    # For Private ip use "networkInterfaces[0].networkIP"
    ansible_host: networkInterfaces[0].accessConfigs[0].natIP
  groups:
    # add hosts to the group 'db' if any of the dictionary's keys or values is the word 'reddit-db'
    db: "'reddit-db' in (tags['items']|list)"
    # add hosts to the group 'app' if any of the dictionary's keys or values is the word 'reddit-app'
    app: "'reddit-app' in (tags['items']|list)"
  ```
  Группы реализованы обоими способами дл/я большей гибкости. Статическое разбиение `groups:` для сохранения обратной совместимости с текущими плейбуками.
* В конфигурационном файле [ansible.cfg](ansible/ansible.cfg) прописано использование динамического инвентаря по-умолчанию
  ```
  [defaults]
  inventory = infra.gcp.yml
  ...

  [inventory]
  enable_plugins = gcp_compute
  ```
* Работа инвентаря протестирована `ansible-inventory --list`
* В шаблоне [db_config.j2](ansible/templates/db_config.j2) в качестве ip-адреса БД установлено значение `['ansible_default_ipv4']['address']` первого инстанса в группе `db`
  ```
  DATABASE_URL={{ hostvars[groups['db'][0]]['ansible_default_ipv4']['address'] }}
  ```
* Реализована группировка хостов в зависимости от значения GCE `labels -> group`, для этого
  * В [terraform/modules/db/main.tf](terraform/modules/db/main.tf) добавлен `labels`
    ```
    labels = {
      group       = "db"
    }
    ```
  * В [terraform/modules/app/main.tf](terraform/modules/app/main.tf) добавлен `labels`
    ```
    labels = {
      group = "app"
    }
    ```
  * В [ansible/infra.gcp.yml](ansible/infra.gcp.yml) блок
    ```
    groups:
      # add hosts to the group 'db' if any of the dictionary's keys or values is the word 'reddit-db'
      db: "'reddit-db' in (tags['items']|list)"
      # add hosts to the group 'app' if any of the dictionary's keys or values is the word 'reddit-app'
      app: "'reddit-app' in (tags['items']|list)"
    ```
    заменён на
    ```
    keyed_groups:
      # Create groups from GCE labels
      - prefix: ""
        separator: ""
        key: labels['group']
    ```

### Провижининг в Packer

* Создан плейбук [packer_db.yml](ansible/packer_db.yml), реализующий провиженинг для образа reddit-db-base
* В [db.json](packer/db.json) провиженер `shell` заменён на `ansible`, запускающий [packer_db.yml](ansible/packer_db.yml)
* В [Makefile](Makefile) добавлена цель `packer_build_db` для сборки packer-образа из [db.json](packer/db.json)
* Собран образ `reddit-db-base`
  ```
  make packer_build_db
  ```
* Создан плейбук [packer_app.yml](ansible/packer_app.yml), реализующий провиженинг для образа reddit-db-base
* В [app.json](packer/app.json) провиженер `shell` заменён на `ansible`, запускающий [packer_app.yml](ansible/packer_app.yml)
* В [Makefile](Makefile) добавлена цель `packer_build_app` для сборки packer-образа из [app.json](packer/app.json)
* Собран образ `reddit-app-base`
  ```
  make packer_build_app
  ```

### Вне задания: Makefile

* Создан [Makefile](Makefile) с набором целей для часто используемых операций
  * `debug` вывод на экран значений переменных
  * `install_packer` скачать и распакова бинарник `packer` в директорию `~/bin/`
  * `install_ansible` установить ansible с зависимостями в python virtualenv
  * `packer_build_db` собрать packer-образ reddit-db-base
  * `packer_build_app` собрать packer-образ reddit-app-base
  * `terraform_stage_init` выполнить terraform init в stage-окружении
  * `terraform_stage_apply` выполнить terraform apply в stage-окружении
  * `terraform_stage_destroy` выполнить terraform destroy в stage-окружении
  * `terraform_stage_url` показать url приложения в stage окружении
  * `terraform_prod_init` выполнить terraform init в prod-окружении
  * `terraform_prod_apply` выполнить terraform apply в prod-окружении
  * `terraform_prod_destroy` выполнить terraform destroy в prod-окружении
  * `terraform_prod_url` показать url приложения в prod окружении
  * `ansible_inventory_list` вывести текущий inventory в json
  * `ansible_site_check` проверить (`--check`) плейбук [site.yml](ansible/site.yml)
  * `ansible_site_apply` выполнить плейбук [site.yml](ansible/site.yml)
  * `build` выполнит `packer_build_db` `packer_build_app`
  * `infra_stage` выполнит `terraform_stage_init` `terraform_stage_apply`
  * `infra_prod` выполнит `terraform_prod_init` `terraform_prod_apply`
  * `site` выполнит `ansible_site_check` `ansible_site_apply`


## HomeWork 10: Ansible: работа с ролями и окружениями

### Основное задание

* Для храниения ролей, создана директория [ansible/roles](ansible/roles)

#### Роль db
* Создана пустая роль `db` с помощью ansible-galaxy
  ```shell
  cd ansible/roles
  ansible-galaxy init db
  ```
  Структура роли
  ```
  $ tree db
  db
  ├── defaults       # <-- Директория для переменных по умолчанию
  │   └── main.yml
  ├── files
  ├── handlers
  │   └── main.yml
  ├── meta           # <-- Информация о роли, создателе и зависимостях
  │   └── main.yml
  ├── README.md
  ├── tasks          # <-- Директория для тасков
  │   └── main.yml
  ├── templates
  ├── tests
  │   ├── inventory
  │   └── test.yml
  └── vars           # <-- Директория для переменных, которые не должны
      └── main.yml   #     переопределяться пользователем

  8 directories, 8 files
  ```
* В задачи роли db [ansible/roles/db/tasks/main.yml](ansible/roles/db/tasks/main.yml) добавлена задача по изменению конфига монги
* Шаблон конфига монги скопирован из [ansible/templates/mongod.conf.j2](ansible/templates/mongod.conf.j2) в [ansible/roles/db/templates/mongod.conf.j2](ansible/roles/db/templates/mongod.conf.j2)
* Определён хэндлер [ansible/roles/db/handlers/main.yml](ansible/roles/db/handlers/main.yml), перезапускающий mongod
* В [ansible/roles/db/defaults/main.yml](ansible/roles/db/defaults/main.yml) определены значения переменных по умолчанию

#### Роль app
* Создана пустая роль `app` с помощью ansible-galaxy
  ```shell
  cd ansible/roles
  ansible-galaxy init app
  ```
* В задачи роли db [ansible/roles/app/tasks/main.yml](ansible/roles/app/tasks/main.yml) добавлены задачи из [ansible/app.yml](ansible/app.yml)
* Шаблон с переменными окружения для запускаемого приложения скопирован из [ansible/templates/db_config.j2](ansible/templates/db_config.j2) в [ansible/roles/app/templates/db_config.j2](ansible/roles/app/templates/db_config.j2)
* Фаил systemd unit-а скопирован из [ansible/files/puma.service](ansible/files/puma.service) в [ansible/roles/app/files/puma.service](ansible/roles/app/files/puma.service)
* В [ansible/roles/app/handlers/main.yml](ansible/roles/app/handlers/main.yml) определён хендлер, перезапускающий сервис `puma`
* В [ansible/roles/app/defaults/main.yml](ansible/roles/app/defaults/main.yml) определена переменная по умолчанию с адресом MongoDB

#### Плейбуки для app и db

* Плейбук [ansible/app.yml](ansible/app.yml) модифицирован на использования роли [ansible/roles/app](ansible/roles/app)
* Плейбук [ansible/db.yml](ansible/db.yml) модифицирован на использования роли [ansible/roles/db](ansible/roles/db)
* Выполнена проверка работоспособности изменённых ролей
  ```shell
  make terraform_stage_destroy terraform_stage_apply
  make ansible_site_check ansible_site_apply
  ```

#### Окружения

* Созданы директории [ansible/environments/stage](ansible/environments/stage) и [ansible/environments/prod](ansible/environments/prod) для соответствующих окружений
* Inventory-файл [ansible/inventory](ansible/inventory) скопирован в директории [ansible/environments/stage](ansible/environments/stage) и [ansible/environments/prod](ansible/environments/prod) и удалён
* Inventory-файл динамического инвентаря [ansible/inventory.gcp.yml](ansible/inventory.gcp.yml) скопирован в директории [ansible/environments/stage](ansible/environments/stage) и [ansible/environments/prod](ansible/environments/prod) и удалён
* **НЕ РАБОТАЕТ** В конфигурационный файл динамического инвентаря [ansible/environments/stage/inventory.gcp.yml](ansible/environments/stage/inventory.gcp.yml) добавлено значение соответствующего окружения
  ```yaml
  compose:
    env: stage
  ```
* Предыдущее действие отменено, для указания окружения, все хосты помещены в группу `gcp_stage`
  ```yaml
  groups:
    gcp_stage: yes
  ```
* **НЕ РАБОТАЕТ** В конфигурационный файл динамического инвентаря [ansible/environments/prod/inventory.gcp.yml](ansible/environments/prod/inventory.gcp.yml) добавлено значение соответствующего окружения
  ```yaml
  compose:
    env: prod
  ```
* Предыдущее действие отменено, для указания окружения, все хосты помещены в группу `gcp_prod`
  ```yaml
  groups:
    gcp_prod: yes
  ```
* В [ansible/ansible.cfg](ansible/ansible.cfg) прописан по умолчанию inventory для stage-окружения
* Изменён [Makefile](Makefile) с набором целей для часто используемых операций. 
  * Добавлена переменная `ENV` для задания окружения. Окружение по умолчанию: `stage`.
  * Добавлена переменная `INV` для задания файла инвентаря. Значение по умолчанию: `inventory.gcp.yml`.
  * В секцию `[inventory]` конфигурационного файла [ansible/ansible.cfg](ansible/ansible.cfg) добавлена поддержка инвентаря в `ini` формате
  ```
  [inventory]
  enable_plugins = gcp_compute, ini
  ```
  * Для запуска цели в prod окружении с использованием статического инвентаря, необходимо выполнить
  ```shell
  make <target> ENV=prod INV=inventory
  ```
* Добавлены `group_vars` для `stage`-окружения
  * [ansible/environments/stage/group_vars/app](ansible/environments/stage/group_vars/app) для группы `app`
  * [ansible/environments/stage/group_vars/db](ansible/environments/stage/group_vars/db) для группы `db`
  * [ansible/environments/stage/group_vars/all](ansible/environments/stage/group_vars/all) для всех групп
* Добавлены `group_vars` для `prod`-окружения
  * [ansible/environments/prod/group_vars/app](ansible/environments/prod/group_vars/app) для группы `app`
  * [ansible/environments/prod/group_vars/db](ansible/environments/prod/group_vars/db) для группы `db`
  * [ansible/environments/prod/group_vars/all](ansible/environments/prod/group_vars/all) для всех групп
* Добавлены значения по умолчанию для переменной `env: local` в каждом из окружений
* В роли [ansible/roles/app](ansible/roles/app) и [ansible/roles/db](ansible/roles/db) добавлена задача, отображающая текущее значение переменной `env`
  ```yaml
  - name: Show info about the env this host belongs to
    debug:
      msg: "This host is in {{ env }} environment!!!"
  ```
* В роли [ansible/roles/app](ansible/roles/app) и [ansible/roles/db](ansible/roles/db) добавлена задача, отображающая текущие группы хоста
  ```yaml
  - name: Show info about groups this host belongs to
    debug:
      msg: "This host is in groups: {{ group_names | join(', ') }}."
  ```
* Выполнена реорганизация файлов и каталогов: <details><summary>подробнее</summary>
  ```
  ansible
  ├── ansible.cfg
  ├── environments
  │   ├── prod
  │   │   ├── group_vars
  │   │   │   ├── all
  │   │   │   ├── app
  │   │   │   └── db
  │   │   ├── inventory
  │   │   └── inventory.gcp.yml
  │   └── stage
  │       ├── group_vars
  │       │   ├── all
  │       │   ├── app
  │       │   └── db
  │       ├── inventory
  │       └── inventory.gcp.yml
  ├── old
  │   ├── files
  │   │   └── puma.service
  │   ├── inventory.json
  │   ├── inventory.yml
  │   ├── json2inv.py
  │   └── templates
  │       ├── db_config.j2
  │       └── mongod.conf.j2
  ├── playbooks
  │   ├── app.yml
  │   ├── clone.yml
  │   ├── db.yml
  │   ├── deploy.yml
  │   ├── packer_app.yml
  │   ├── packer_db.yml
  │   ├── reddit_app_multiple_plays.yml
  │   ├── reddit_app_one_play.yml
  │   └── site.yml
  ├── requirements.txt
  └── roles
      ├── app
      │   ├── defaults
      │   │   └── main.yml
      │   ├── files
      │   │   └── puma.service
      │   ├── handlers
      │   │   └── main.yml
      │   ├── meta
      │   │   └── main.yml
      │   ├── README.md
      │   ├── tasks
      │   │   └── main.yml
      │   ├── templates
      │   │   └── db_config.j2
      │   ├── tests
      │   │   ├── inventory
      │   │   └── test.yml
      │   └── vars
      │       └── main.yml
      └── db
          ├── defaults
          │   └── main.yml
          ├── files
          ├── handlers
          │   └── main.yml
          ├── meta
          │   └── main.yml
          ├── README.md
          ├── tasks
          │   └── main.yml
          ├── templates
          │   └── mongod.conf.j2
          ├── tests
          │   ├── inventory
          │   └── test.yml
          └── vars
              └── main.yml

  28 directories, 46 files
  ```
  <details>
* Улучшен конфиг [ansible/ansible.cfg](ansible/ansible.cfg)
  * Явно указан путь к ролям
    ```ini
    roles_path = ./roles
    ```
  * Включен обязательный вывод diff при наличии изменений и вывод 5 строк контекста
    ```ini
    [diff]
    always = True
    context = 5
    ```
  * Добавлены комментарии

#### Проверка
* Уничтожено окружение `stage`
  ```shell
  make ENV=stage terraform_destroy
  ```
* Создано окружение `prod`
  ```shell
  make ENV=prod terraform_apply
  ```
* Развёрнут сайт
  ```shell
  make ENV=prod ansible_site_apply
  ```
* Проверена работоспособность (в браузере открыт url)
  ```shell
  make terraform_url ENV=prod
  ```
* Без уничтожения prod-окружения, создано `stage` окружение
  ```shell
  make ENV=stage terraform_apply
  make ENV=stage ansible_site_apply
  make ENV=stage terraform_url
  ```
* При проверкe `stage` окружения, возникла ошибка подключения к БД. Причиной оказалась **ошибка** при назначении переменной
  ```
  DATABASE_URL={{ hostvars[groups['db'][0]]['ansible_default_ipv4']['address'] }}
  ```
  берётся ip-адрес первого хоста в группе `db`, который принадлежит другому окружению и имеет другой ip
  TODO: продумать решение данной проблемы!
* Уничтожена инфраструктура окружения `prod`
  ```shell
  make ENV=prod terraform_destroy
  ```
* Повторно развёрнут сайт на `stage`-окружении
  ```shell
  make ENV=stage ansible_site_apply
  ```
* При тестировании снова возникла ошибка доступа к БД. В [ansible/roles/app/tasks/main.yml](ansible/roles/app/tasks/main.yml) в задачу `Add config for DB connection` добавлено уведомление хендлера, перезапускающего сервис puma: `notify: reload puma`, после чего сервис был вручную перезапущен из консоли
  ```shell
  cd ./ansible && ../.venv/bin/ansible -i environments/stage/inventory.gcp.yml app --become -m systemd -a "name=puma state=restarted"
  ```

#### Работа с Community-ролями

* Создан файл с зависимостями для `prod` [ansible/environments/prod/requirements.yml](ansible/environments/prod/requirements.yml) и `stage` [ansible/environments/stage/requirements.yml](ansible/environments/stage/requirements.yml) окружений, содержащий модуль `jdauphant.nginx`
  ```yaml
  - src: jdauphant.nginx
    version: v2.21.1
  ```
* Создана цель в [Makefile](Makefile)
  ```shell
  ansible_install_requirements:
  	cd ./ansible && ../.venv/bin/ansible-galaxy install -r environments/${ENV}/requirements.yml
  ```
* Установлена роль `jdauphant.nginx` с `ansible-galaxy`
  ```shell
  make ansible_install_requirements
  ```
* Конфигурация для роли добавлена в переменные группы `app` обоих окружений
  ```yaml
  nginx_sites:
  default:
    - listen 80
    - server_name "reddit"
    - location / {
      proxy_pass http://127.0.0.1:9292;
      }
  ```
* В [terraform/modules/app/main.tf](terraform/modules/app/main.tf) добавлено правило фаервола `modules.app.google_compute_firewall.firewall_http` для пропуска трафика на 80 порт хостов с меткой `reddit-app`
* В плейбук [ansible/playbooks/app.yml](ansible/playbooks/app.yml) добавлен вызов роли `jdauphant.nginx`
* В плейбук [ansible/playbooks/deploy.yml](ansible/playbooks/deploy.yml) добавлен вывод url сайта (порт по умолчанию, `80`)
* Инфраструктура `stage` создана, плейбук `site.yml` выполнен, работоспособность сайта проверена
  ```shell
  make terraform_apply ansible_site_apply
  ```

#### Ansible vault

* Создан файл с ключём вне репозирория. Данный файл прописан в [ansible/ansible.cfg](ansible/ansible.cfg)
  ```ini
  vault_password_file = ~/path/to/vault.key
  ```
* Создан плейбук [ansible/playbooks/users.yml](ansible/playbooks/users.yml), добавляющий пользователей в систему
* Созданы файлы с credentials для stage и prod окружений
  * [ansible/environments/stage/credentials.yml](ansible/environments/stage/credentials.yml)
  * [ansible/environments/prod/credentials.yml](ansible/environments/prod/credentials.yml
* Файлы с credentials зашифрованы
  ```shell
  cd ansible
  ansible-vault encrypt environments/stage/credentials.yml
  ansible-vault encrypt environments/prod/credentials.yml
  ```
* Вызов плейбука `users.yml` добавлен в основной плейбук [ansible/playbooks/site.yml](ansible/playbooks/site.yml)
* Проверена работоспособность `make terraform_apply ansible_site_apply`
* После включения авторизации в ssh с использованием пароля (а не только ключа), удалось успешно подключиться пользователем `admin`

### Задание со \*: Использование динамического инвернтаря

Уже реальзовано на стадии создания окружений

### Задание с \*\*: Настройка TravisCI

#### Подготовка

* Исправлены пути к провиженерам в
  * [packer/ubuntu16.json](packer/ubuntu16.json)
  * [packer/immutable.json](packer/immutable.json)
* В [Makefile](Makefile) добавлена цель `terraform_validate`, выполняющая `terraform validate` в директориях
  * [terraform/](terraform/)
  * [terraform/](terraform/stage)
  * [terraform/](terraform/prod)
* В [Makefile](Makefile) добавлена цель `install_terraform`, выполняющая установку `terraform`
* В [Makefile](Makefile) добавлена цель `install_tflint`, выполняющая установку `tflint`
* В [Makefile](Makefile) добавлена цель `terraform_tflint`, выполняющая проверку средствами `tflint` следующих директорий
  * [terraform/](terraform/)
  * [terraform/stage](terraform/stage)
  * [terraform/prod](terraform/prod)
* Создан конфигурационный файл [terraform/.tflint.hcl](terraform/.tflint.hcl) с описанием конфига `tflint`. Ссылка на [документацию](https://github.com/wata727/tflint/blob/master/docs/guides/config.md)
* В [Makefile](Makefile) добавлена цель `ansible_lint`, выполняющая проверку всех [ansible-плейбуков](ansible/playbooks) средствами `ansible-lint`
* В [ansible/requirements.txt](ansible/requirements.txt) добавлена зависимость `ansible-lint==4.1.0`
* Исправлены предупреждения линтера:
  * В [ansible/.ansible-lint](ansible/.ansible-lint) добавлено исключение директории [ansible/roles_imported/](ansible/roles_imported/) из проверки линтером
  * Заполнена мета-информация ролей
    * [ansible/roles/app/meta/main.yml](ansible/roles/app/meta/main.yml)
    * [ansible/roles/ви/meta/main.yml](ansible/roles/ви/meta/main.yml)
  * Добавлена версия git-репозитория в [ansible/playbooks/clone.yml](ansible/playbooks/clone.yml)
* В [Makefile](Makefile) добавлена цель `ansible_syntax`, выполняющая проверку синтаксиса всех [ansible-плейбуков](ansible/playbooks)
* Настроен [trytravis](https://github.com/sethmlarson/trytravis) в соответствии с [инструкцией](https://medium.com/@Nklya/локальное-тестирование-в-travisci-2b5ef9adb16e)
* Исправлен путь к ролям в [ansible/ansible.cfg](ansible/ansible.cfg) с  целью прохождения travis-ci тестов. С `roles_path = ./roles_imported:./roles` на `roles_path = ./roles`
* С той же целью изменён [.gitignore](.gitignore)
* В [Makefile](Makefile) добавлены две цели
  ```
  install: install_packer install_terraform install_tflint install_ansible
  validate: packer_validate terraform_validate terraform_tflint ansible_syntax ansible_lint
  ```
* Доработан [Makefile](Makefile). Пути к исполняемым файлам `packer`, `terraform`, `tflint`, `ansible` теперь можно задать через переменные окружения
* В [Makefile](Makefile) добавлена цель `terraform_init_nobackend` для инициализации terraform без использования remote backends. Необходимо для статической валидации средствами `terraform validate`
* В [Makefile](Makefile) добавлена цель `install_ansible_virtualenv` для установки ansible в virtualenv-окружение с использованием пакета `virtualenv`
* В [Makefile](Makefile) добавлено отображение версий используемых программ при вызове линтеров
* В [Makefile](Makefile) для `ansible_syntax` явно указан inventory-файл [ansible/environments/stage/inventory](ansible/environments/stage/inventory) чтобы избежать предурпеждений во время проверки синтаксиса

#### Trytravis

* В [README.md](README.md) добавлен статус билда, как описано в [документации](https://docs.travis-ci.com/user/status-images)
* Создан пустой репозиторий [trytravis-otus](https://github.com/vscoder/trytravis-otus), содержащий только `README.md`. Имя репозитория должно содержать `trytravis`
* В [https://travis-ci.org](https://travis-ci.org) (обязательно **.org**) выполнен вход по учётке github
* Добавлен созданный репозиторий
* Для настройки trytravis на локальном хосте выполнена команда `trytravis --repo ssh://git@github.com/vscoder/trytravis-otus.git`, указывающая использовать данный репозиторий для тестирования
* Для запуска тестирования, необходимо перейти в директорию тестируемого репозитория и запустить `trytravis`
  ```shell
  cd vscoder-infra
  trytravis
  ```

#### Реализация

* В [.travis.yml](.travis.yml) реализована валидация кода packer и terraform. А именно
  * Добавлена секция `install` с установкой необходимых бинарников
    ```yaml
    install:
      - make install_packer install_terraform install_tflint
    ```
  * Добавлена секция `before_script` с действиями, подготавливающими код к валидации
    ```yaml
    before_script:
      # Создание файлов-заглушек с переменными
      - cp packer/variables.json.example packer/variables.json
      - cp terraform/terraform.tfvars.example terraform/terraform.tfvars
      - cp terraform/stage/terraform.tfvars.example terraform/stage/terraform.tfvars
      - cp terraform/prod/terraform.tfvars.example terraform/prod/terraform.tfvars
      # Инициализация terraform для директории terraform/, а так же для stage и prod окружений
      - make terraform_init_nobackend ENV=""
      - make terraform_init_nobackend ENV="stage"
      - make terraform_init_nobackend ENV="prod"
    ```
  * Добавлена секция `script`, в которой выполняется валидация
    ```yaml
    script:
      - make packer_validate terraform_validate terraform_tflint
    ```
* Создан скрипт-обёртка [packer/scripts/ansible-playbook.sh](packer/scripts/ansible-playbook.sh) для запуска packer-ом провиженера типа ansible
  В шаблонах packer-а [packer/app.json](packer/app.json) и [packer/db.json](packer/db.json) в провиженер типа ansible добавлен параметр `command`, указывающий на созданный скрипт. Теперь провиженеры выглядят так (пример для [db.json](packer/db.json))
  ```json
  "provisioners": [
    {
      "type": "ansible",
      "command": "packer/scripts/ansible-playbook.sh",
      "playbook_file": "ansible/playbooks/packer_db.yml"
    }
  ]
  ```
* В [.travis.yml](.travis.yml) для ansible-плейбуков добавлена проверка синтаксиса и запуск `ansible-lint`
  ```yaml
  script:
    # ...
    - make ansible_syntax ansible_lint
  ```


## HomeWork 11: Разработка и тестирование Ansible ролей и плейбуков

### Локальная разработка при помощи Vagrant, доработка ролей для провижининга в Vagrant

#### Установка Vagrant

* Установлен VirtualBox 6.0.14
* Установлен Vagrant `Vagrant 2.2.6`

* В [.gitignore](.gitignore) добавлены относящиеся к vagrant и molecule временные файлы
  ```
  ####
  # Vagrant & molecule
  ####
  .vagrant/
  *.log
  *.pyc
  .molecule
  .cache
  .pytest_cache
  ```

* Добавлен [ansible/Vagrantfile](ansible/Vagrantfile) с описанием terraform-инфраструктуры в vagrant (2 ВМ, db и app)
* Установлен VirtualBox
* Выполнен `vagrant up`
  <details><summary>CLICK ME</summary>
  <p>

  ```
  Bringing machine 'dbserver' up with 'virtualbox' provider...
  Bringing machine 'appserver' up with 'virtualbox' provider...
  ==> dbserver: Box 'ubuntu/xenial64' could not be found. Attempting to find and install...
      dbserver: Box Provider: virtualbox
      dbserver: Box Version: >= 0
  ==> dbserver: Loading metadata for box 'ubuntu/xenial64'
      dbserver: URL: https://vagrantcloud.com/ubuntu/xenial64
  ==> dbserver: Adding box 'ubuntu/xenial64' (v20191024.0.0) for provider: virtualbox
      dbserver: Downloading: https://vagrantcloud.com/ubuntu/boxes/xenial64/versions/20191024.0.0/providers/virtualbox.box
      dbserver: Download redirected to host: cloud-images.ubuntu.com
  ==> dbserver: Successfully added box 'ubuntu/xenial64' (v20191024.0.0) for 'virtualbox'!
  ==> dbserver: Importing base box 'ubuntu/xenial64'...
  ==> dbserver: Matching MAC address for NAT networking...
  ==> dbserver: Checking if box 'ubuntu/xenial64' version '20191024.0.0' is up to date...
  ==> dbserver: Setting the name of the VM: ansible_dbserver_1572247326926_10235
  Vagrant is currently configured to create VirtualBox synced folders with
  the `SharedFoldersEnableSymlinksCreate` option enabled. If the Vagrant                                                                                                           
  guest is not trusted, you may want to disable this option. For more                                                                                                              
  information on this option, please refer to the VirtualBox manual:                                                                                                               

    https://www.virtualbox.org/manual/ch04.html#sharedfolders                                                                                                                      

  This option can be disabled globally with an environment variable:                                                                                                               

    VAGRANT_DISABLE_VBOXSYMLINKCREATE=1                                                                                                                                            

  or on a per folder basis within the Vagrantfile:                                                                                                                                 

    config.vm.synced_folder '/host/path', '/guest/path', SharedFoldersEnableSymlinksCreate: false                                                                                  
  ==> dbserver: Clearing any previously set network interfaces...
  ==> dbserver: Preparing network interfaces based on configuration...
      dbserver: Adapter 1: nat
      dbserver: Adapter 2: hostonly
  ==> dbserver: Forwarding ports...
      dbserver: 22 (guest) => 2222 (host) (adapter 1)
  ==> dbserver: Running 'pre-boot' VM customizations...
  ==> dbserver: Booting VM...
  ==> dbserver: Waiting for machine to boot. This may take a few minutes...
      dbserver: SSH address: 127.0.0.1:2222
      dbserver: SSH username: vagrant
      dbserver: SSH auth method: private key
      dbserver: 
      dbserver: Vagrant insecure key detected. Vagrant will automatically replace
      dbserver: this with a newly generated keypair for better security.
      dbserver: 
      dbserver: Inserting generated public key within guest...
      dbserver: Removing insecure key from the guest if it's present...
      dbserver: Key inserted! Disconnecting and reconnecting using new SSH key...
  ==> dbserver: Machine booted and ready!
  ==> dbserver: Checking for guest additions in VM...
      dbserver: The guest additions on this VM do not match the installed version of
      dbserver: VirtualBox! In most cases this is fine, but in rare cases it can
      dbserver: prevent things such as shared folders from working properly. If you see
      dbserver: shared folder errors, please make sure the guest additions within the
      dbserver: virtual machine match the version of VirtualBox you have installed on
      dbserver: your host and reload your VM.
      dbserver: 
      dbserver: Guest Additions Version: 5.1.38
      dbserver: VirtualBox Version: 6.0
  ==> dbserver: Setting hostname...
  ==> dbserver: Configuring and enabling network interfaces...
  ==> dbserver: Mounting shared folders...
      dbserver: /vagrant => /mnt/calculate/home/vscoder/projects/otus/devops201908/vscoder_infra/ansible
  ==> appserver: Box 'ubuntu/xenial64' could not be found. Attempting to find and install...
      appserver: Box Provider: virtualbox
      appserver: Box Version: >= 0
  ==> appserver: Loading metadata for box 'ubuntu/xenial64'
      appserver: URL: https://vagrantcloud.com/ubuntu/xenial64
  ==> appserver: Adding box 'ubuntu/xenial64' (v20191024.0.0) for provider: virtualbox
  ==> appserver: Importing base box 'ubuntu/xenial64'...
  ==> appserver: Matching MAC address for NAT networking...
  ==> appserver: Checking if box 'ubuntu/xenial64' version '20191024.0.0' is up to date...
  ==> appserver: Setting the name of the VM: ansible_appserver_1572247362999_16688
  ==> appserver: Fixed port collision for 22 => 2222. Now on port 2200.
  ==> appserver: Clearing any previously set network interfaces...
  ==> appserver: Preparing network interfaces based on configuration...
      appserver: Adapter 1: nat
      appserver: Adapter 2: hostonly
  ==> appserver: Forwarding ports...
      appserver: 22 (guest) => 2200 (host) (adapter 1)
  ==> appserver: Running 'pre-boot' VM customizations...
  ==> appserver: Booting VM...
  ==> appserver: Waiting for machine to boot. This may take a few minutes...
      appserver: SSH address: 127.0.0.1:2200
      appserver: SSH username: vagrant
      appserver: SSH auth method: private key
      appserver: 
      appserver: Vagrant insecure key detected. Vagrant will automatically replace
      appserver: this with a newly generated keypair for better security.
      appserver: 
      appserver: Inserting generated public key within guest...
      appserver: Removing insecure key from the guest if it's present...
      appserver: Key inserted! Disconnecting and reconnecting using new SSH key...
  ==> appserver: Machine booted and ready!
  ==> appserver: Checking for guest additions in VM...
      appserver: The guest additions on this VM do not match the installed version of
      appserver: VirtualBox! In most cases this is fine, but in rare cases it can
      appserver: prevent things such as shared folders from working properly. If you see
      appserver: shared folder errors, please make sure the guest additions within the
      appserver: virtual machine match the version of VirtualBox you have installed on
      appserver: your host and reload your VM.
      appserver: 
      appserver: Guest Additions Version: 5.1.38
      appserver: VirtualBox Version: 6.0
  ==> appserver: Setting hostname...
  ==> appserver: Configuring and enabling network interfaces...
  ==> appserver: Mounting shared folders...
      appserver: /vagrant => /mnt/calculate/home/vscoder/projects/otus/devops201908/vscoder_infra/ansible
  ```

  </p>
  </details>
* Краткий список команд
  * Проверка что бокс скачан `vagrant box list`
  * Посмотреть список запущенных ВМ `vagrant status`
  * Подключиться к ВП по ssh `vagrant ssh VMNAME`
  * Запустить провиженер `vagrant provision [VMNAME]`

#### Доработка ролей

##### Provisioning

* Добавлен провиженер в [ansible/Vagrantfile](ansible/Vagrantfile) ВМ `db`
  ```ruby
  db.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbooks/site.yml"
    ansible.groups = {
    "db" => ["dbserver"],
    "db:vars" => {"mongo_bind_ip" => "0.0.0.0"}
    }
  end
  ```
* Запущен провиженер `vagrant provision dbserver`
* Возникла ошибка:
  ```
  fatal: [dbserver]: FAILED! => {"changed": false, "msg": "Could not find the requested service mongod: host"}
  ```
  Причина -- роль [ansible/roles/db](ansible/roles/db) писалась с учётом базового packer-образа с уже установленной MongoDB
* В роль [ansible/roles/db](ansible/roles/db) добавлены задачи по установке MongoDB
* Провиженинг завершён успешно
* Добавлен плейбук [ansible/playbooks/base.yml](ansible/playbooks/base.yml) для установки python если он не установлен. Ошибки не было, но того требуют автоматизированные тесты

* Задачи роли [ansible/roles/db](ansible/roles/db) из [ansible/roles/db/tasks/main.yml](ansible/roles/db/tasks/main.yml) разнесены по файлам
  * Задачи по установке MongoDB вынесены в [ansible/roles/db/tasks/install_mongodb.yml](ansible/roles/db/tasks/install_mongodb.yml)
  * Задачи по настройке MongoDB вынесены в [ansible/roles/db/tasks/config_mongodb.yml](ansible/roles/db/tasks/config_mongodb.yml)
* Для проверки, повторно выполнен провиженинг. Прошёл успешно
  
* Задачи роли [ansible/roles/app](ansible/roles/app) из [ansible/roles/app/tasks/main.yml](ansible/roles/app/tasks/main.yml) разнесены по файлам
  * Задачи по установке MongoDB вынесены в [ansible/roles/app/tasks/ruby.yml](ansible/roles/app/tasks/ruby.yml)
  * Задачи по настройке MongoDB вынесены в [ansible/roles/app/tasks/puma.yml](ansible/roles/app/tasks/puma.yml)
* Добавлен провиженер в [ansible/Vagrantfile](ansible/Vagrantfile) ВМ `app`
  ```ruby
  db.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbooks/site.yml"
    ansible.groups = {
    "db" => ["appserver"],
    "app:vars" => { "db_host" => "10.10.10.10"}
    }
  end
  ```
* Запущен провиженер `vagrant provision appserver`. Возникла ошибка:
  ```
  TASK [app : Add config for DB connection] **************************************
  fatal: [appserver]: FAILED! => {"changed": false, "checksum": "dfbe4b5cf3ec32d91d20045e2ee7f7b26c60ef34", "msg": "Destination directory /home/appuser does not exist"}
  ```
* Для исправления ошибки, параметризована роль [ansible/roles/app](ansible/roles/app)
  * В переменные по умолчанию [ansible/roles/app/defaults/main.yml](ansible/roles/app/defaults/main.yml) добавлен `deploy_user: appuser`
  * [ansible/roles/app/files/puma.service](ansible/roles/app/files/puma.service) перемещён в [ansible/roles/app/templates/puma.service.j2](ansible/roles/app/templates/puma.service.j2)
  * В шаблоне [ansible/roles/app/templates/puma.service.j2](ansible/roles/app/templates/puma.service.j2) все упоминания пользователя `appuser` заменены на переменную `{{ deploy_user }}`
  * В [ansible/roles/app/tasks/puma.yml](ansible/roles/app/tasks/puma.yml) все упоминания пользователя `appuser` заменены на переменную `{{ deploy_user }}`
* Так же захаржкоженный `appuser` заменён на `{{ deploy_user }}` в [ansible/playbooks/deploy.yml](ansible/playbooks/deploy.yml)
* В [ansible/Vagrantfile](ansible/Vagrantfile) добавлено переопределение переменных дл япровиженера
  ```ruby
  config.vm.define "appserver" do |app|
    ...

    app.vm.provision "ansible" do |ansible|
      ...
      ansible.extra_vars = {
        "deploy_user" => "ubuntu"
      }
    end
  end
  ```
* Запущен провиженер `vagrant provision appserver`. Прошёл успешно

* Проверена работа приложения [http://10.10.10.20:9292/](http://10.10.10.20:9292/). Успешно.
* Конфигурация пересоздана, перепроверена и удалена
  ```shell
  vagrant destroy -f
  vagrant up
  #open in browser http://10.10.10.20:9292/
  vagrant destroy -f
  ```

#### Задание со \*: Прлксирование средствами nginx

##### Исследование

* Диагностика показала, что для nginx отсутствует конфиг, описанный в [ansible/environments/stage/group_vars/app](ansible/environments/stage/group_vars/app) в переменной `nginx_sites`
* Причина: Vagrant, для прогона плейбуков, использует свой inventory `.vagrant/provisioners/ansible/inventory/vagrant_ansible_inventory`, в котором не учитываются значения переменных inventory из репозитория
* Есть 2 варианта решения проблемы: 
  * прописать переменные непосредственно в `Vagrantfile`
  * указать путь к инвентори параметром `ansible.inventory_path`

##### Реализация

* Был выбран первый способ, как наиболее оптимальный по временным затратам
  ```ruby
  ansible.extra_vars = {
    "deploy_user" => "ubuntu",
    "nginx_sites" => {
      "default" => [
        "listen 80",
        "server_name \"reddit\"",
        "location / {
          proxy_pass http://127.0.0.1:9292;
        }"
      ]
    }
  }
  ```
* Результат проверен. Сайт открывается по адресу [http://10.10.10.20](http://10.10.10.20)

### Тестирование ролей при помощи Molecule и Testinfra

* В [ansible/requirements.txt](ansible/requirements.txt) добавлены зависимости от:
  ```
  ...
  molecule>=2.6
  testinfra>=1.10
  python-vagrant>=0.5.15
  ```
* Зависимости установлены `make install_ansible_venv`
* Создание заготовки тестов `cd ansible/roles/db && molecule init scenario --scenario-name default --role-name db --driver-name vagrant`
* В [ansible/roles/db/molecule/default/tests/test_default.py](ansible/roles/db/molecule/default/tests/test_default.py) добавлены 2 теста
  ```python
  # check if MongoDB is enabled and running
  def test_mongo_running_and_enabled(host):
      mongo = host.service("mongod")
      assert mongo.is_running
      assert mongo.is_enabled

  # check if configuration file contains the required line
  def test_config_file(host):
      config_file = host.file('/etc/mongod.conf')
      assert config_file.contains('bindIp: 0.0.0.0')
      assert config_file.is_file
  ```
* Создана ВМ для проверки роли `cd ansible/roles/db && molecule create`
* Список созданных инстансов `cd ansible/roles/db && molecule list`
* Подключиться к инстансу по ssh `cd ansible/roles/db && molecule login -h instance`

* В molecule-плейбук [ansible/roles/db/molecule/default/playbook.yml](ansible/roles/db/molecule/default/playbook.yml) до бавлены `become` и переменные
  ```yaml
  ...
  become: true
  ...
  vars:
    mongo_bind_ip: 0.0.0.0
  ...
  ```
* Проверка выполнения роли [ansible/roles/db/molecule/default/playbook.yml](ansible/roles/db/molecule/default/playbook.yml) `cd ansible/roles/db && molecule converge`
* Прогон тестов из [ansible/roles/db/molecule/default/tests/test_default.py](ansible/roles/db/molecule/default/tests/test_default.py) `cd ansible/roles/db && molecule verify`

* Докупентация по [testinfra](https://testinfra.readthedocs.io/en/latest/modules.html)
* В тесты [ansible/roles/db/molecule/default/tests/test_default.py](ansible/roles/db/molecule/default/tests/test_default.py) добавлена проверка, что MongoDB слушает на порту 27017
  ```python
  # check mongod is listening on 0.0.0.0:27017
  def test_mongo_socket(host):
      socket = host.socket("tcp://0.0.0.0:27017")
      assert socket.is_listening
  ```

### Переключение сбора образов пакером на использование ролей

* Документация по конфигурированию ansible через переменные среды [https://docs.ansible.com/ansible/latest/reference_appendices/config.html](https://docs.ansible.com/ansible/latest/reference_appendices/config.html)

#### Провиженинг в db.json
* При импорте задачь в [ansible/roles/db/tasks/main.yml](ansible/roles/db/tasks/main.yml) добавлены соответствующие теги
  ```yaml
  - import_tasks: install_mongodb.yml
    tags:
      - db_install_mongodb

  - import_tasks: config_mongodb.yml
    tags:
      - db_configure_mongodb
  ```
* В [плейбуке](ansible/playbooks/packer_db.yml), используемом при провижениенге пакер-образа db, использована роль вместо списка задач
  ```yaml
  ...
  roles:
    - db
  ```
* В шаблоне пакер-образа [packer/db.json](packer/db.json) в секцию `provisioners` добавлено 2 параметра:
  ```json
  "provisioners": [
    {
      "type": "ansible",
      "command": "packer/scripts/ansible-playbook.sh",
      "playbook_file": "ansible/playbooks/packer_db.yml",
      "ansible_env_vars": [
        "ANSIBLE_ROLES_PATH=./ansible/roles"
      ],
      "extra_arguments": [
        "--tags",
        "db_install_mongodb"
      ]
    }
  ]
  ```
  * `ansible_env_vars` указан путь к ролям **относительно корня репозитория**
  * `extra_arguments` плейбуку передаётся агрумент `--tags` с указание обязательных тегов, которые должны присутствовать на задачах

#### Провиженинг в app.json
* При импорте задачь в [ansible/roles/app/tasks/main.yml](ansible/roles/app/tasks/main.yml) добавлены соответствующие теги
  ```yaml
  - import_tasks: ruby.yml
    tags:
      - app_ruby

  - import_tasks: puma.yml
    tags:
      - app_puma
  ```
* В [плейбуке](ansible/playbooks/packer_app.yml), используемом при провижениенге пакер-образа app, использована роль вместо списка задач
  ```yaml
  ...
  roles:
    - app
  ```
* В шаблоне пакер-образа [packer/app.json](packer/app.json) в секцию `provisioners` добавлено 2 параметра:
  ```json
  "provisioners": [
    {
      "type": "ansible",
      "command": "packer/scripts/ansible-playbook.sh",
      "playbook_file": "ansible/playbooks/packer_app.yml",
      "ansible_env_vars": [
        "ANSIBLE_ROLES_PATH=./ansible/roles"
      ],
      "extra_arguments": [
        "--tags",
        "app_ruby"
      ]
    }
  ]
  ```
  * `ansible_env_vars` указан путь к ролям **относительно корня репозитория**
  * `extra_arguments` плейбуку передаётся агрумент `--tags` с указание обязательных тегов, которые должны присутствовать на задачах

### Задание со \*: Подключение Travis CI для автоматического прогона тестов

#### Вынесение роли в отдельный репозиторий
##### Подготовка репозитория
* Создан GitHub-репозиторий [ansible-role-db](https://github.com/vscoder/ansible-role-db)
  **важно**: название должно начинаться с `ansible-role-`, иначе будут сложности с тестированием
* Созданный пустой репозиторий склонирован в `../ansible-role-db`
* Созержимое [ansible/roles/db](ansible/roles/db) перенесено в `../ansible-role-db`
* Заполнен `../ansible-role-db/README.md`
* Создан `../ansible-role-db/Makefile`
* При попытке выполнить `molecule converge` не удалось най ти роль `db`.
  **Исправлена** приведением файла `../ansible-role-db/molecule/default/playbook.yml` к следующему содержимому:
  ```yaml
  ---
  - name: Converge
    become: true
    hosts: all
    vars:
      mongo_bind_ip: 0.0.0.0
    roles:
      - role: "{{ lookup('env', 'MOLECULE_PROJECT_DIRECTORY') | basename }}"
  ```
  Выражение `{{ lookup('env', 'MOLECULE_PROJECT_DIRECTORY') | basename }}` позволяет в качестве имени роли использовать basename текущей директории.
  **ссылки по теме**
  * [ANSIBLE_RIOLES_PATH](https://github.com/ansible/molecule/blob/fc90dfd6c8a5fd3a3068b9cc8311dc176ab261cd/molecule/provisioner/ansible.py#L203-L208) где molecule ищет роли
  * [github issue](https://github.com/ansible/molecule/issues/1567#issuecomment-436876722)
* В `../ansible-role-db/README.md` добавлено описание целей `../ansible-role-db/Makefile`
* Текущей ревизии назначен тег `git tag v0.1`
* Выполнен пуш репозитория в GitHub, включая теги `git push --tags`

##### Переход на использование внешней роли
* В зависимости [ansible/environments/stage/requirements.yml](ansible/environments/stage/requirements.yml) и [ansible/environments/prod/requirements.yml](ansible/environments/prod/requirements.yml) добавлена созданная роль
  ```yaml
  - name: vscoder.db
    src: https://github.com/vscoder/ansible-role-db
    version: v0.1
  ```
* Роль добавлена в [.gitignore](.gitignore)
* Выполнена установка зависимостей
  ```shell
  make ansible_install_requirements
  ```
  вывод
  ```
  cd ./ansible && ../.venv/bin/ansible-galaxy install -r environments/stage/requirements.yml
  - jdauphant.nginx (v2.21.1) is already installed, skipping.
  - extracting vscoder.db to /mnt/calculate/home/vscoder/projects/otus/devops201908/vscoder_infra/ansible/roles/vscoder.db
  - vscoder.db (v0.1) was installed successfully
  ```
* Плейбук [ansible/playbooks/db.yml](ansible/playbooks/db.yml) переделан на использование новой роли
  ```yaml
  - name: Configure MongoDB
    hosts: db
    become: true
    vars:
      mongo_bind_ip: 0.0.0.0
    roles:
      - vscoder.db
  ```
* Выполнено пробное развёртывание stage-окружения
  При попытке открыть сайт, возникла ошибка подключения к БД.
  Причина - изменение [ansible/roles/app/templates/db_config.j2](ansible/roles/app/templates/db_config.j2) в commit e8d9303b22b238f78b1ab40f2162ca9166545949
* Содержимое [ansible/roles/app/templates/db_config.j2](ansible/roles/app/templates/db_config.j2) исправлено на
  ```jinja
  {% if env == 'local' %}
  DATABASE_URL={{ db_host }}
  {% elif env in ['stage', 'prod'] %}
  DATABASE_URL={{ hostvars[groups['db'][0]]['ansible_default_ipv4']['address'] }}
  {% endif %}
  ```
  В случае запуска в локальном окружении, значение переменной перётся из переменной `db_host`. Иначе получается динамически с первого хоста в группе `db`
  commit 8c47a5c4764dac915581fcc8363a30ab11309311
* Развёртывание прошло успешно.

* При попытке собрать packer-образ, возникла ошибка об отсутствии роли `db`
  Исправил
  ```yaml
  - name: Configure MongoDB
    hosts: all
    become: true
    roles:
      - vscoder.db
  ```

#### Автоматизированное тестирование в travic-ci внешней роли db средствами molecule в gce

Пример роли https://github.com/Artemmkin/test-ansible-role-with-travis

* Создан ssh-ключ `ssh-keygen -t rsa -f google_compute_engine -C 'travis' -q -N ''`
* Публичный ключ добавлен в  проект infra в gcp средствами terraform
  * в файл [terraform/terraform.tfvars](terraform/terraform.tfvars) в список `ssh_keys`
* Чтобы добавить ключ, применена инфраструктура `cd terraform && terraform apply`
* Создан сервис-аккаунт (IAM & admin -> Service accounts) `ci-test`
  * Присвоена роль `Compute Admin`
  * После <details><summary>ошибки</summary>
    <p>
    The user does not have access to service account '973349678085-compute@developer.gserviceaccount.com'.  User: 'travis-ci@infra-253214.iam.gserviceaccount.com'.  Ask a project owner to grant you the iam.serviceAccountUser role on the service account
    <p>
    </details>
    Присвоена роль `Service Account User`
  * json-ключ сохранён в `../ansible-role-db/credentials.json`
  * **ВАЖНО** Изменения применяются не сразу, после создания нового аккаунта или изменения списка ролей должно пройти некоторое время (5-10мин, но это не точно)
* **ПРИМЕЧАНИЕ** Для отключения опции `no_log` при создании инстанса, нужно в плейбуке `molecule/gce/create.yml` добавить переменную `molecule_no_log` в секцию `vars`. При желании, можно реализовать через переменную окружения.
* **ПРИМЕЧАНИЕ** Все подробности по созданию инстанса можно посмотреть в плейбуке `molecule/gce/create.yml`
* В `../ansible-role-db/.travis.yml` добавлены переменные окружения в **зашифрованном** виде
  ```shell
  travis encrypt GCE_SERVICE_ACCOUNT_EMAIL='travis-ci@infra-253214.iam.gserviceaccount.com' --add
  travis encrypt GCE_CREDENTIALS_FILE='${PWD}/credentials.json' --add
  travis encrypt GCE_PROJECT_ID='infra-253214' --add
  ```
* Зашифрованы файлы
  ```shell
  tar cvf secrets.tar credentials.json google_compute_engine
  travis login
  travis encrypt-file secrets.tar --add
  ```
* Удалось добиться успешного подключения к GCE во время билда (первая стадия `destroy`), после указания в секретный переменных пути к файлам в текущей директории через `${PWD}`
* Но возникла ошибка на стадии `create`
* В `../ansible-role-db/.travis.yml` добавлена переменная `USER`
* Содержимое `../ansible-role-db/.travis.yml` после всех можификаций (исключены секреты)
  <details><summary>.travis.yml</summary>
  
  ```yaml
  ...
  install:
  - pip install ansible==2.8.6 molecule[gce] apache-libcloud
  script:
    - ls -la
    - molecule --debug test --scenario-name gce
  after_script:
    - molecule destroy --scenario-name gce
  before_install:
    - openssl aes-256-cbc -K $encrypted_<generate_automatically>_key -iv $encrypted_<generate_automatically>_iv
      -in secrets.tar.enc -out secrets.tar -d
    - tar xvf secrets.tar
    - mv google_compute_engine /home/travis/.ssh/
    - chmod 0600 /home/travis/.ssh/google_compute_engine
  env:
    global:
      - USER=travis
      - secure: ...
      ...
  ```

  </details>
* По окончании всех тестов, отключен вывод отладочной информации при выполнении тестов `molecule`
* Обновлена версия роли до v0.2
* Обновлены зависимости stage-окружения [ansible/environments/stage/requirements.yml](ansible/environments/stage/requirements.yml). Обновлена версия требуемой роли
  ```yaml
  - name: vscoder.db
    src: https://github.com/vscoder/ansible-role-db
    version: v0.2
  ```

#### Прочие изменения

* В [ansible/ansible.cfg](ansible/ansible.cfg) настроена загрузка внешних ролей в [ansible/roles_imported](ansible/roles_imported)
* 

# Makefile

## Переменные

### Общие
`BIN_DIR` директория с исполняемыми файлами (или директория для распаковки исполняемых файлов) packer, terraform, tflint. По умолчанию `~/bin`
`TEMP_DIR` временная директория для загрузки packer, terraform, tflint. По умолчанию `/tmp`
`ENV` окружение, stage или prod. По умолчанию `stage`
`INV` имя inventory-файла ansible в директории соответствующего окружения

### Packer
`PACKER_VERSION` версия packer. По умолчанию `1.4.4`
`PACKER` путь к исполняемому файлу packer. По умолчанию `${BIN_DIR}/packer`

### Terraform
`TERRAFORM_VERSION` версия terraform. По умолчанию `0.12.12`
`TERRAFORM` путь к исполняемому файлу terraform. По умолчанию `${BIN_DIR}/terraform`

### Tflint
`TFLINT_VERSION` версия tflint. По умолчанию `0.12.1`
`TFLINT` путь к исполняемому файлу tflint. По умолчанию `${BIN_DIR}/tflint`

### Ansible
`ANSIBLE` путь к исполняемому файлу ansible относительно директории `./ansible`. По умолчанию `../.venv/bin/ansible`. Для использования system-wide ansible, необходимо присвоить `ANSIBLE=ansible`

## Цели

`debug` вывод на экран значений переменных

### Устанока зависимостей
`install_packer` скачать и распакова исполняемый файл `packer` в директорию `~/bin/`
`install_ansible_virtualenv` установить ansible с зависимостями в виртуальное окружение python с использованием `virtualenv`. Подходит для старых дистрибутивов с python2 (протестировано на ubuntu-14.04)
`install_ansible_venv` установить ansible с зависимостями в виртуальное окружение python с использованием `python3 -m venv`. Подходит для современных дистрибутивов с python3.5+ (протестировано на ubuntu-18.04)
`install_terraform` скачать и распакова исполняемый файл `terraform` в директорию `~/bin/`
`install_tflint` скачать и распакова исполняемый файл `tflint` в директорию `~/bin/`

### Packer
`packer_build_db` собрать packer-образ reddit-db-base
`packer_build_app` собрать packer-образ reddit-app-base
`packer_validate` выполнить валидацию шаблонов packer

### Terraform
`terraform_init ENV=<stage|prod>` выполнить terraform init
`terraform_init_nobackend ENV=<stage|prod>` выполнить terraform init без проверки remote backends (для последующей валидации кода)
`terraform_apply ENV=<stage|prod>` выполнить terraform apply
`terraform_destroy ENV=<stage|prod>` выполнить terraform destroy
`terraform_url ENV=<stage|prod>` показать url приложения

### Ansible
`ansible_inventory_list ENV=<stage|prod>` вывести текущий inventory в json
`ansible_install_requirements ENV=<stage|prod>` установить внешние роли из `environments/${ENV}/requirements.yml`
`ansible_lint` выполнить `ansible-lint` для всех плейбуков в [ansible/playbooks](ansible/playbooks)
`ansible_site_check` выполнить `ansible-playbook --syntax-check` для всех плейбуков в [ansible/playbooks](ansible/playbooks)
`ansible_site_check ENV=<stage|prod>` проверить (`--check`) плейбук [site.yml](ansible/playbooks/site.yml)
`ansible_site_apply ENV=<stage|prod>` выполнить плейбук [site.yml](ansible/playbooks/site.yml)

### Vagrant
`vagrant_up` поднять боксы вагрант из [ansible/Vagrantfile](ansible/Vagrantfile)

### Aliases
`install`: `install_packer install_terraform install_tflint install_ansible_venv`
`validate`: `packer_validate terraform_validate terraform_tflint ansible_syntax ansible_lint`
`build`: `packer_build_db packer_build_app`
`infra`: `terraform_init terraform_apply`
`site`: `ansible_site_check ansible_site_apply`
