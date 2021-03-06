***[ Команда git add](./add.md)*** <== ***[Содержание](./readme.md)*** ==> ***[ Команда git amend](./amend.md)***

## Команда git commit

---


`git commit` фиксирует изменения. Эти коммиты представляют собой снимки всего вашего репозитория в определенное время. Каждый раз когда вы что-то меняете в своём проекте следует делайть новый коммит. Со временем коммиты должны рассказывать историю вашего репозитория и то, как он стал таким, какой он есть сейчас. В дополнение к содержимому и сообщению коммиты включают множество метаданных, таких как автор, временная метка и т. д.

Что бы зафиксировать внесённые  изменения нужно написать команду: `git commit -m «commit comment»`


```
$ git commit -m "Story 182: fix benchmarks for speed"
[master 463dc4f] Story 182: fix benchmarks for speed
 2 files changed, 2 insertions(+)
 create mode 100644 README
```

Вы можете видеть, что коммит вывел вам немного информации о себе: на какую ветку вы выполнили коммит (master), какая контрольная сумма SHA-1 у этого коммита (463dc4f), сколько файлов было изменено, а также статистику по добавленным/удалённым строкам в этом коммите.

Запомните, что коммит сохраняет снимок состояния вашего индекса. Всё, что вы не проиндексировали, так и висит в рабочем каталоге как изменённое; вы можете сделать ещё один коммит, чтобы добавить эти изменения в репозиторий. Каждый раз, когда вы делаете коммит, вы сохраняете снимок состояния вашего проекта, который позже вы можете восстановить или с которым можно сравнить текущее состояние.

---