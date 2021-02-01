# Шпаргалка по командам git

[< к содержанию](../readme.md)

## Таблица команд и их значение в кратком виде.
<br>

| Значение команды | Наименование команды              
| -------------    |:------------------:| 
| Создать новый репозиторий       | `git init project-name`    |    
| Добавить файл в репозиторий     | `git add text.txt`         |
| Удалить файл:                   | `git rm text.txtt`         |
| Текущее состояние репозитория   | `git status`               |
| Сделать коммит                  | `git commit -a -m "Commit description"`         |
| Запушить текущую ветку, не вводя целиком ее название    | `git push origin HEAD`         |
| Создать новый бранч             | `git branch some_branch`         |
| Переключиться на другую ветку   | `git checkout some_branch`         |
| Получаем список веток, с которыми работаем    | `git branch`         |
| Просмотреть все существующие ветви    | `git branch -a`         |
| Удалить бранч (после мержа)     | `git branch -d some_branch`         |
| Просто удалить бранч            | `git branch -D some_branch`         |
| История изменений               | `git log`         |
| История изменений в обратном порядке    | `git log --reverse`         |
| История конкретного файла       | `git log file.txt`         |
| Удалить бранч из репозитория на сервере  | `git push origin :branch-name`         |
| Создание глобального файла .gitignore    | `git config --global core.excludesfile ~/.gitignore_global`         |
| Создание тэга                   | `git tag some_tag`         |
| Удаление untracked files        | `git clean -f`         |
<br>

