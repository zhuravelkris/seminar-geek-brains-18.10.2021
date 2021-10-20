
# Инструкция по работе с Git и GitHub 

Это краткая инструкция по работе с Git и GitHub, в которой будут рассмотрены основные термины, самые распространненные команды для работы с репозиториями. Помимо этого остановимся на работе с популярным сервисом  для хранения репозиториев GitHub, а так же на том, как передавать информацию от локального репозитория к удаленному и обратно, работать с репозиториями других авторов и отправлять запросы на редактуру в чужих репозиториях. 

## Что такое система контроля версий 

Система контроля версий - это программное обеспечение для облегчения работы с изменяющейся информацией. Система управления версиями позволяет хранить несколько версий одного и того же документа, при необходимости возврщаться к более ранним версиям, определять, кто и когда сделал то или иное изменение и многое другое. 


## Что такое git 

Git - это одна из реализаций распределенных систем контроля версий. Git позволяет управлять изменениями, создавать фиксации, ветки, а также сливать и удалять ветки.

## Подготовка репозитория 

Репозиторий - это хранилище файлов, поддерживающее версионность. Создать репозиторий можно с помощью команды *git init* 


## Создание сохранений 

Мы можем создавать "сохранения" наших версий файлов. Такие "сохранения" называются фиксациями или коммитами. Сделать коммит можно с помощью команды *git commit* и **ОБЯЗАТЕЛЬНО** использовать флаг *-m*, после чего в кавычках написать сообщение.

## Журнал изменений 


## Перемещение между сохранениями 

Перемещаться между нашими сохранениями можно с помощью команды *git checkout*. Для этого достаточно применить команду *git checkout <номер коммита>*. 

Можно отменить изменения с помощью команд *git revert* и *git reset*.

*git revert <номер коммита>* отменит изменения до указнной версии и создаст новый коммит. 

*git reset --hard <номер коммита>* отменит изменения до указанной версии и сотрет всю историю изменений после этого коммита.


## Ветки 

Новая ветка создается с помощью команды *git branch <название ветки>* 


## Слияние веток и решение конфликтов 

Слияние веток происходит с помощью команды *git merge*. Для слияния содержимого другой ветки в текущую необходимо использовать команду *git merge <название ветки>*. Если возникнет конфликт, его необходимо разрешить. 

## Удаление веток 

Удалить уже слитую ветку мы можем с помощью команды *git branch -d*. Для этого необходимо написать git branch -d <имя ветки>

## Скачивание удаленного репозитория 

Для получения копии существующего Git-репозитория, например, проекта, в который вы хотите внести свой вклад, необходимо использовать команду *git clone*. 

Клонирование репозитория осуществляется командой *git clone <url>*. Например, если вы хотите клонировать библиотеку *libgit2*, вы можете сделать это следующим образом:

  > $ git clone https://github.com/libgit2/libgit2

Эта команда создаёт каталог libgit2, инициализирует в нём подкаталог .git, скачивает все данные для этого репозитория и извлекает рабочую копию последней версии. Если вы перейдёте в только что созданный каталог *libgit2, то увидите в нём файлы проекта, готовые для работы или использования.

## Отправка изменений в удаленный репозиторий 
Для отправки изменений в удаленный репозиторий используется команда *git push* Для этого пишется в папке с репозиторием команда *git push origin <название ветки>*. Чаще всего используется ветка мастер 


## Pull Requests 

Для принятия изменений из ветки в ветку в нашем репозитории, или из форка удаленного репозитория, используются Pull Requests.
