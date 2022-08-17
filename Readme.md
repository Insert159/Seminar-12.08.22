# Инструкция по работе с GIT и ветками

## Что такое GIT
GIT - одна из реализаций систем контроля версий, позволяющая реализовать версионность, как локально, так и на удалённом сервере. Самая популярная платформа реализующая Git - [GitHub](https://github.com)

## Подготовка репозитория
Для создания в папке репозитория необходимо открыть эту папку в терминале и написать команду *git init* ПОСЛЕ ЧЕГО В ЭТОЙ ПАПКЕ СОЗДАСТСЯ СКРЫТАЯ ПАПКА *.GIT* и таким образом папка станет репозиторием

## Создание коммитов

### Создание фиксаций
Для создания фиксаций используется команда *Git commit*, для этого в папке репозитория необходимо написать кроманду *git commit -m <сообщение к комиту>*. сООБЩЕНИЕ К КОММИТУ ПИСАТЬ обязательно

### Просмотр состояния репозитория
Для простомра состояния репозитория используется команда *git status*, в терминале с открытой папкой-репозиторием необходимо написать команду *git status*. В результате можно видеть следующие выводы
1. On branch *** nothing to commit - это означает нет активных изменений 
2. Untreacked file - это означает, что имеются файлы, не отслеживаемые системой контроя версий
...

## Добавление файла к коммиту
для того чтобы добавить файл к сохранению необходимо использовать команду *Git add*, в терминале с открытой папкой-репозиторием необходимо написать *git add <название файла>*, и этот файл добавить к сохранению

## Журнал изменений
Для просмотра историй изменений используется команда *git log*, для этого в терминале с папкой-репозиторием необходимо написать *git log* и вы увидете список всех коммитов в этой ветке с описанием имени, электронной почты, сообщением коммиту и номер коммита.

## Перемещение между коммитами
Для перемещения между коммитами используется команда *git checkout*. Для этогов терминале с папкой-репозиторием необходимо написать *git checkout <номер коммита>*. Номер коммита берется из журнала изменений ветки

## Ветки в GIT
### Создание ветки
для того, чтобы создать новую ветку, используется команда *git branch*, для этого в терминале папки- репозитория необходимо написать команду *git branch <имяВетки>*. И таким образом создасться новая ветка, но вы останетесь в исходной 

### Переключение между ветками
Для того, чтобы переключиться на другую ветку используется команда *git checkout*, для этого в терминале папки-репозитория используется команда *git checkout <название ветки>* и тгда вы перейдете на другую ветку. Для переключения между ветками ветка должна существовать, а на текущей ветки не должно быть активных изменений

для создания новой ветки в *git* необходимо набрать команду *git branch <название ветки>*. Командой *git branch* можно простотреть все созданные ветки. Текущая ветка помечена символом *.

## Слияние веток и решение конфликтов
Силяние веток в *git*. В терминале с папкой-репозиторием необходимо написать *git merge <имя ветки для слияния>*. Важный момент. Необходимо быть на ветке к коморой мы маржируем. 

Конфликты при слиянии веток решается вручную или я еще не всё знаю про git. Сейчас создам конфликт и проверю. А вот и он

## Удаление веток
Удаление веток в *GIT* происходит через команду *git branch -d <имя ветки>*
Удаление происходит безвозвратно!!! 


Всем хорошего дня!
