# Команда git push

Команда **git push** при выполнении перемещает изменения, внесенные пользователем на локальном компьютере, в удаленный репозиторий. После того как пользователи клонировали удаленный репозиторий и внесли необходимые изменения в свое локальное устройство, эти изменения должны быть перенесены в удаленный репозиторий. Причина в том, что они являются общими и используются другими пользователями. Команда **git push** делает это. Эти изменения представляют собой обязательства, выполненные в репозитории, а не незафиксированные изменения (если таковые имеются).

Кроме того, изменения, которые пользователь вносит в локальную систему, не имеют никакой ценности для участников и зрителей, если облако GitHub не отражает их.

Чтобы иметь возможность перейти в удаленный репозиторий, вы должны убедиться, что все ваши изменения в локальном репозитории зафиксированы.

Рассмотрим **git push** как часть процесса синхронизации в Git. Синхронизация происходит между локальным и удаленным хранилищем, где источник и приемник могут отличаться. Есть много других частей для синхронизации, и **git push**-это одна из частей, потому что она загружает изменения, сделанные в локальном репозитории, чтобы поддерживать удаленный репозиторий в актуальном состоянии. В этом нет ничего сложного, и концепция проста, как и ее синтаксис.

- Пользователь клонирует репозиторий в качестве первого шага, чтобы внести некоторые изменения в репозиторий.

- После этого он приступает к внесению изменений в локальную систему и добавляет эти изменения в промежуточную область.

- После завершения всех изменений пользователь затем фиксирует все изменения в локальном репозитории.

- А затем передает эти изменения на удаленный сервер. Наконец, он синхронизирует локальный и удаленный репозитории.

## Синтаксис команды git Push в Git
***
Выполнение команды **git push** происходит путем ввода следующей команды:

`git push <remote_repo> <branch_name>`

**remote_repo**: это имя (или псевдоним) удаленного репозитория, в который мы переносим изменения.

**branch_name**: это ветвь, которую пользователь толкает в удаленный репозиторий.

Представьте себе, что ветвь (branch) в Git подобна ветвям в дереве. Каждая ветвь представляет собой новую функцию или модификацию, находящуюся в стадии разработки. Кроме того, основная ветвь — это стабильный код, подобный стволу дерева, также называемый _master branch_ (главной ветвью). Что, в свою очередь, помогает нестабильному коду ветвей держаться подальше от стабильного основного кода.

## Варианты Git Push
***

В **git push command** доступно множество опций, которые помогают нам достичь определенных конкретных задач всего за одно выполнение. В этом разделе мы рассмотрим основные и наиболее часто используемые параметры команды **git push**.

### Prune Option

— опция prune в команде **git push** удалит ветвь XYZ из удаленного репозитория, если в локальном репозитории не существует ветви с таким же именем.

_Использование_: `git push –prune remote XYZ`

### Dry Run Option

Эта опция будет выполнять и показывать выполнение команды **git push**, но не будет отправлять никаких обновлений в удаленный репозиторий.

_Использование_: `git push –dry-run <remote> <local_branch> `
### Atomic Option

Эта опция в **git Push** обеспечивает атомарную операцию на удаленном репозитории, т. е. либо каждую ссылку обновляет, либо вообще ничего.

_Использование_: `git push –atomic <remote_repo> <working_branch>`
### All Option

Все опции будут выталкивать все ветви и их зафиксированные изменения в удаленный репозиторий.

_Использование_: `git push-all <remote>`
