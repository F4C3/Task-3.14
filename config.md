***[Установка](./install.md)*** <== ***[Содержание](./readme.md)*** ==> ***[Команда git init](./init.md)***

## Команда git config

---

В состав Git входит утилита `git config` , которая позволяет просматривать и настраивать параметры, контролирующие все аспекты работы Git, а также его внешний вид. 


Чтобы посмотреть все установленные настройки и узнать где именно они заданы, используйте команду:

`$ git config --list --show-origin`


Первое, что вам следует сделать после установки Git - указать ваше имя и адрес электронной почты. Это важно, потому что каждый коммит в Git содержит эту информацию, и она включена в коммиты, передаваемые вами, и не может быть далее изменена:

`$ git config --global user.name "John Doe"`

`$ git config --global user.email johndoe@example.com`


Если вы хотите проверить используемую конфигурацию, можете использовать команду `git config --list`, чтобы показать все настройки, которые Git найдёт:

```
$ git config --list
user.name=John Doe
user.email=johndoe@example.com
color.status=auto
color.branch=auto
color.interactive=auto
color.diff=auto
...
```

---