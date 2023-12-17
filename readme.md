# Инструкция по работе с GIT

LICENSE: [MIT](/licenses/license.md)

![GIT logo](/images/Git-logo-black.svg)

---
## Содержание
1. [Что такое GIT?](./whatisgit.md)
2. [Как работает GIT?](./howgitworks.md)
3. [Установка GIT](./setup.md)
4. [Настройка](./setting.md)
5. [Создание репозотирия](./createrepository.md)
6. [Определение состояния](./status.md)
7. [Подготовка файлов](./preparefiles.md)
8. [Фиксация изменений](./fixchanges.md)
    * [Как сделать коммит?](./fixchanges.md#как-сделать-коммит)
    * [Как посмотреть коммиты?](./fixchanges.md#как-посмотреть-коммиты)
9. [Удалённые репозитории](./remoterepository.md)
    * [Что такое удалённый репозиторий?](./remoterepository.md#что-такое-удалённый-репозиторий)
    * [Подключение к удалённому репозиторию](./remoterepository.md#подключение-к-удалённому-репозиторию)
    * [Отправка изменений на сервер](./remoterepository.md#отправка-изменений-на-сервер)
    * [Запрос изменений с сервера](./remoterepository.md#запрос-изменений-с-сервера)
10. [Ветвление](./branches.md)
    * [Создание новой ветки](./branches.md#создание-новой-ветки)
    * [Переключение между ветками](./branches.md#переключение-между-ветками)
    * [Слияние веток](./branches.md#слияние-веток)
    * [Как удалять ветки в GIT?](./branches.md#как-удалять-ветки-в-git)
11. [Настройка *.gitignore*](./gitignore.md)
    * [Какие файлы нужно исключать?](./gitignore.md#какие-файлы-нужно-исключить)
    * [Правила синтаксиса файла *.gitignore*](./gitignore.md#правила-синтаксиса-файла-gitignore)
    * [Комментарии](./gitignore.md#комментарии)
    * [Рассечение](./gitignore.md#рассечение)
    * [Литеральные имена файлов](./gitignore.md#литеральные-имена-файлов)
    * [Знаки подстановки](./gitignore.md#знаки-подстановки)
    * [Квадратные скобки](./gitignore.md#квадратные-скобки)
    * [Файлы, которые не нужно исключать](./gitignore.md#файлы-которые-не-нужно-исключать)
    * [Как исключить файлы, которые уже отслеживаются?](./gitignore.md#как-исключить-файлы-которые-уже-отслеживаются)
    * [Просмотр всех игнорируемых файлов](./gitignore.md#просмотр-всех-игнорируемых-файлов)
12. [Основные команды GIT](./basicgitcommands.md)
    * [git add](./basicgitcommands.md#git-add)
    * [git status](./basicgitcommands.md#git-status)
    * [git diff](./basicgitcommands.md#git-diff)
    * [git commit](./basicgitcommands.md#git-commit)
    * [git reset](./basicgitcommands.md#git-reset)
    * [git rm](./basicgitcommands.md#git-rm)
    * [git mv](./basicgitcommands.md#git-mv)
    * [git clean](./basicgitcommands.md#git-clean)
    * [git branch](./basicgitcommands.md#git-branch)
    * [git checkout](./basicgitcommands.md#git-checkout)
    * [git merge](./basicgitcommands.md#git-merge)
    * [git log](./basicgitcommands.md#git-log)
    * [git tag](./basicgitcommands.md#git-tag)
    * [git fetch](./basicgitcommands.md#git-fetch)
    * [git pull](./basicgitcommands.md#git-pull)
    * [git push](./basicgitcommands.md#git-push)
    * [git remote](./basicgitcommands.md#git-remote)

---
GIT logo by Jason Long - http://git-scm.com/downloads/logos,
LICENSE: [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/deed.ru) 