[<< К содержанию](./readme.md)

## Ветвление

Во время разработки нового функционала считается хорошей практикой работать с копией рабочего проекта, которую называют **веткой**

### Создание новой ветки

Для создания новой ветки используется команда:

```bash hljs=
git branch <name_of_new_branch>
```
это создаст новую ветку, пока что точную копию основной ветки.

### Переключение между ветками

Чтобы переключаться между ветками нужно использовать команду:

```bash hljs=
git checkout <name_of_branch>
```

### Слияние веток

Разработка над новым функционалом завершена. Необходимо внести изменения в выбранную ранее ветку:

```bash hljs=
git add <path_of_filename>
git commit -m "New feature complete"
```

После этого можно переключиться на главную ветку:

```bash hljs=
git checkout master
```

Чтобы внести изменения в главную ветку, необходимо произвести слияние веток:

```bash hljs=
git merge <name_of_branch>
```

где **<name_of_branch>** - название ветки, с которой нужно слить главную ветку.

После этого ветку **<name_of_branch>** можно удалить:

```bash hljs=
git branch -d <name_of_branch>
```

Для создания копии удалённого репозитория нужно использовать команду `git clone`:

```bash hljs=
git clone <url_of_github_repository>
```

### Как удалять ветки в GIT?

```bash hljs=
git branch -d <name_of_branch>
```

Удалить текущую ветку, которая просматривается в данный момент - нельзя. При попытке это сделать, система выдаст ошибку. Поэтому при удалении ветки, необходимо сначала преключиться на другую ветку.
