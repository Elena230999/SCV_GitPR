# Репозиторий для **pull request**
* В своём аккаунте на GitHub создать копию репозитория **"AndreyBulgakov19/SCV_GitPR"** с помощью кнопки **"Fork"**.
---
* Клонировать копию репозитория на локальный компьютер.
---
* Создать новую ветку.
---
* Добавить файл с инструкцией в новую ветку.
---
* Дополнить инструкцию разделами по работе с удалёнными репозиториями, pull request.
---
* Зафиксировать изменения (коммиты).
---
* Отправить изменения на GitHub.
---
* На сайте GitHub выполнить **Pull request**.
---
# Work with Git
## 1. Проверка Git
Проверяем, работает ли Git командой **git version**. Если git установлен, появится сообщение с информацией о версии программы, иначе будет сообщение об ошибке.

## 2. Установка git
Загружаем последнюю версию программы с [сайта](https://git-scm.com/downloads). Устанавливаем с настроками по умолчанию.

## 3. Настройка git
Первое, что вам следует сделать после установки Git — указать ваше имя и адрес электронной почты. Это важно, потому что каждый коммит в Git содержит эту информацию, и она включена в коммиты, передаваемые вами, и не может быть далее изменена:

*git config --global user.name "John Doe"*

*git config --global user.email johndoe@example.com*
## 4. Инициализация репозитория
Инициализация репозитория Git производится командой **git init** в директории проекта. При этом директория может содержать файлы проекта или быть пустой.

После инициализации репозитория в директории проекта будет создана скрытая поддиректория .git, которая содержит различные сущности Git и информацию о репозитории.
## 5. Запись изменений в репозиторий
Для записи изменений в репозиторий Git используйте следующие команды:

**Git add** — добавляет все изменённые файлы в рабочей директории в индекс.

**Git commit** — сохраняет изменения в истории коммитов. Каждый коммит в Git имеет уникальный идентификатор, дату и время коммита, имя автора, электронную почту и сообщение, описывающее изменения.
## 6. Просмотр истории коммитов
Для просмотра истории предыдущих коммитов в обратном хронологическом порядке можно использовать команду **git log**
## 7. Перемещение между сохранениями (коммитами)
Для перехода в другой коммит надо ввести команду **git checkout [номер коммита]**.

Чтобы вернуться в исходное состояние, надо ввести команду **git checkout main**
## 8. Игнорирование файлов
Для того, чтобы исключить отслеживание в репоззитории определенные файлы и папки, необходимо сознать файл **.gitignore** и записать в него их названия или шаблоны, соответствующие таким файлам или папкам.

## 9. Создание веток в git
По умолчанию имя основной ветки **main** 
Создать ветку можно командой *git branch <name>*
*git checkot <name>* - переключаемся между ветками
## 10. Слияние веток
Сливаются ветки командой *git merge «text»*, при этом нужно находиться в основной ветке, в которую нужно влить фиче-ветку.
## 11. Разрешение конфликтов
Необходимо проанализировать входящие изменения и выбрать пожходящее нам.
## 12. Удаление веток
Чтобы удалить ветку из локального Git-репозитория, выполните: **git branch -d <имя_ветки>**
## 13. Работа с удаленными репозиториями
1. Создайте новый репозитори на GitHub;
2. Создать локальный репозиторий
3. Содать удаленный репозиторий
4. Связать локальный репозиторий с удаленным
* Настройте подключение к удаленному репозиторию через HTTPS;
* С помощью команды **git clone <url-адрес репозитория>** осуществите клонирование внешнего репозитория на локальный ПК;
* Создайте в файле новую ветку, чтобы вносить изменения;
* Команда **git pull** позволяет  получить изменения и слияние с локальной версией;
* Команда **git push** отправляет локальную версию репозитория на внешний

Мы создали удаленный репозиторий, узнали про подключение удаленного репозитория, рассмотрели команды clone, push, pull для взаимодействия с ним.