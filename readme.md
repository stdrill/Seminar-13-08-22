# Инструкция по работе с Git

## Что такое *git*

*Git* - одна из реализаций распределенных систем контроля версий, позволяющая организовать версионность, как локально, так и на удаленном сервере. Самая популярная платформа, реализующая Git - [GitHub](https//:github.com)

## Подготовка репозитория

Для создания в папке репозитория необходимо открыть эту папку в терминале и написать команду *git init*, после чего в этой папке появится скрытая папка *.git* и, таким образом, папка станет репозиторием.

## Создание коммитов

Для создания фиксаций используется команда *git commit*. Для этого в терминале с репозиторием необходимо написать команду *git commit -m <сообщение к коммиту>. Сообщение к коммиту писать обязательно.

## Просмотр состояния репозитория

Для просмотра состояния репозитория используется команда *git status*. В терминале с открытой папкой-репозиторием необходимо написать команду *git status*. В результате можно увидеть следующие выводы:
1. On branch *** Nothing to commit - нет активных изменений
2. Untracked files - файлы, неотслеживаемые системой контроля версий

## Добавление файла к сохранению

Для того чтобы добавить файл к сохранению, необходимо использовать команду *git add*. В терминале с открытой папкой-репозиторием необходимо написать git add <название файла>, и этот файл добавится к сохранению.

## Журнал изменений

Для просмотра журнала изменений используется команда *git log*. Для это в терминале с папкой-репозиторием необходимо написать *git log*. В терминале отобразятся все совершенные коммиты с комментариями.

## Перемещение между коммитами
Для перемещения между коммитами используется команда *git checkout*. Для этого в терминале с папкой-репозиторием необходимо написать *git checkout <номер коммита>*. Номер коммита берется из журнала изменений ветки.

## Ветки в Git

Для создания новой ветки используется команда *git branch <имя ветки>*. Для этого в терминале с папкой-репозиторием необходимо написать *git branch <имя ветки>*.

Для просмотра всех существующих веток необходимо в терминале написать команду *git branch*.

## Перемещение между ветками

Для перемещения между ветками в терминале необходимо ввести команду *git checkout <название ветки>*.

## Слияние веток и решение конфликтов

Для слияния веток необходимо в терминале ввести команду *git merge <имя ветки>*. Слияние должно происходить из основной ветки к которой сливаются все остальные.

В случае если в сливаемой ветке были внесены изменения в данные из основной ветки, возникает конфликт. Самый простой способ разрешить конфликт — отредактировать конфликтующий файл. 

## Удаление веток

Для удаления ветки необходимо в терминале ввести команду *git branch -d <имя ветки>*.