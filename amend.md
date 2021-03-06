***[ Команда git commit](./commit.md)*** <== ***[Содержание](./readme.md)*** ==> ***[ Команда git reset](./reset.md)***


## Команда git commit --amend


---


Команда `git commit --amend` — это удобный способ изменить последний коммит. Она позволяет объединить проиндексированные изменения с предыдущим коммитом без создания нового коммита. Ее можно использовать для редактирования комментария к предыдущему коммиту без изменения состояния кода в нем. Но такое изменение не только редактирует последний коммит, но и полностью его заменяет. То есть измененный коммит станет новой сущностью с отдельной ссылкой. Для Git он будет выглядеть как новый коммит. Существует несколько распространенных сценариев использования команды `git commit --amend`.

```
 $ git commit --amend -m "an updated commit message"
 ```

Допустим, при выполнении коммита вы допустили ошибку в комментарии к нему. Выполнение этой команды в отсутствие проиндексированных файлов позволяет отредактировать комментарий к предыдущему коммиту без изменения состояния кода.

В процессе разработки регулярно случаются преждевременные коммиты. Очень просто забыть проиндексировать файл или использовать неправильный формат комментария к коммиту. Флаг `--amend` позволяет удобно исправить эти небольшие ошибки.

```
 $ git commit --amend --no-edit
```

Флаг `--no-edit` позволит внести изменения в коммит без изменения комментария к нему. Итоговый коммит заменит неполный коммит. При этом все будет выглядеть так, словно изменения в файлах были сделаны за один коммит.

---