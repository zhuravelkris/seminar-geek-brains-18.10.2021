
# Инструкция по работе с Git и GitHub 

## Что такое система контроля версий 



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


## Отправка изменений в удаленный репозиторий 
Для отправки изменений в удаленный репозиторий используется команда *git push* Для этого пишется в папке с репозиторием команда *git push origin <название ветки>*. Чаще всего используется ветка мастер 