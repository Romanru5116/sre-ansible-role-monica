Whats New:
20/11
1 переработан task - использованы blocks
2 отформатированы отступы
3 assert уточнены
4 добавлен шаблон hosts.yml

Ничего не тестировалось, нужна Centos у меня Ubuntu.
Просьба: если есть устоявшиеся правила шаблонного оформления кода роли ли или шагов тестирования - дать их  как пример единообразия.
 Спасибо 
----

05/11
Подправлено название роли в /sre-ansible-role-monica/molecule/default/playbook.yml тэг import_role на корректное
04/11
--- Ничего не проверялось -----
сделано описание решения  в документе по ходу решения этой учебной задачи
Поправлен сам код Ansible - добавлена работа с Centos
Исправлен основной конфиг молекулы - для php7 указан контейнер для разверрывания с Centos 7
Исправлен файл converge - теперь туда включено описание роли
----------
ранее
изменен сам код (папка tasks/main.yml) - под Rpm пакеты - Centos в частности. По сравнению с имеющимся базовым кодом c apt пришлось задействовать встроенный модуль ANSIBLE - ansible.builtin.dnf, ; сделать проверку что эта ОС Centos;  как это все заживет в реальности не понимаю- честно скажу - ключи репозитория, завиcbмости пакетов и  molecule - это новые вещи для меня


=========
[![Galaxy](https://img.shields.io/badge/galaxy-kevit.monica-blue.svg?style=flat)](https://galaxy.ansible.com/kevit/monica)
[![Build Status](https://travis-ci.org/kevit/ansible-role-monica.svg?branch=master)](https://travis-ci.org/kevit/ansible-role-monica)

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

| Name              | Default Value       | Description          |
|-------------------|---------------------|----------------------|
| `` | `` |  |

Переменные используются внутренние  
Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

    - hosts: all
      roles:
         - kevit.monica

License
-------

Apache 2.0
