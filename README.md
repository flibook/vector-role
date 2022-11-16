Vector
=========

Учебная Ansible роль для установки [Vector](https://vector.dev)

Requirements
------------

Поддержка Debian и RPM систем (писалась для Ubuntu Focal и CentOS 7, по идее и на других должна работать)

Role Variables
--------------

| Переменная | Тип | Значение по умоланию | Комментарий |
| --- | --- | --- | --- |
| `vector_version` | Строка | 0.21.1 | Номер версии vector |

Dependencies
------------

Зависимостей нет

Example Playbook
----------------

```yml
- name: Install Vector
  hosts: vector
  roles:
    - vector
```

License
-------

MIT
