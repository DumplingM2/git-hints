# git-hints

## Небольшой гит-репозиторий для самостоятельной работы

`git clone https://github.com/PraktikumJava/git-hints.git`

Статусы файлов
В Git файлы могут находиться в нескольких статусах:

untracked: файл не отслеживается Git и не включён в коммиты.
modified: файл изменён, но изменения не добавлены в индекс.
staged: файл добавлен в индекс с помощью git add и готов для коммита.
committed: изменения сохранены в коммите и включены в историю.

```mermaid
graph LR;
untracked -- "git add" --> staged;
staged -- "git commit" --> committed;
committed -- "изменения" --> modified;
modified -- "git add" --> staged;
```