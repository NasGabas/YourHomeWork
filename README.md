# Добрый день, уважаемые студенты! 
  При выполнении данной работы от вас требуется дополнить мой репозиторий, добавив в него свой файл с инструкцией по работе с git. Помните, что добавление файла - такой же процесс изменения репозитория, как и изменения внутри конкретных файлов и не пугайтесь этого :)

  P.S. Называйте добавляемые файлы своими фамилиями(только на английской раскладке), чтобы мне было проще их идентифицировать. И не забудьте сделать скрин окна с pullrequest, на сайт GB необходимо отослать именно этот скрин, чтобы работа была окончательно завершена.

  P.P.S. Не забывайте, что отправляем на pullrequest мы побочные ветки!

  # Конспект Габасовой Анастасии

  # Введение в контроль версий.

## Знакомство с контролем версий.

**Контроль версий нужен для:**
1. хранения различных версий проекта
2. возможности возвращаться к различным версиям проекта

**GIT** - программа, которая осуществляет порядок системы контроля версий. 

Создатель GIT - Линус Торвальдс.

> Программа GIT сохраняет в памяти не файлы целиком, а разницу между исходным и последущим файлами.

## Четыре шага внесения изменений

| Шаги | Расшифровка |
| :---- | :---- |
| изменяем информацию | вносим в редактор информацию |
| сохраняем информацию | ctrl + s |
| добавляем измененные файлы к отслеживанию | git add |
| фиксируем изменения | git commit -m |

## Синтаксис языка Markdown

| Форма выделения | Особенности выделения
| :---- | :---- |
| **Жирный текст** | обрамление двойными звездочками (**) |
| *Курсив* | обрамление одной звездочкой (*) |
| Выделение заголовка | решетка в начале строки (#) |


# Инструкция по работе в Git

## Первый семинар. Первое использование контроля версий.

### Основные команды 

* *git init* - команда, инициализирующая репозиторий в заданной директории.

* *git checkout* - команда, которая задает выбор необходимой сохраненной версии файла.

* *git commit* - команда, которая фиксирует изменения в файле.

* *git add* - команда, которая добавляет изменения файла к отслеживанию.

* *git log* - команда, которая выводит полный список изменений, с указанием дат, времени и автора изменений.

* *git diff* - команда, которая помогает найти разницу между репозиториями /файлами.

## Второй семинар. Второе использование контроля версий. Установка и настройка системы контроля версий. 

### Создание веток

* *git branch* - команда, которая вызывает все существующие ветки в репозитории.

* *git branch + name* - команда, которая позволяет создавать новые ветки с именем.

* *git checkot + name* - команда, которая позволяет перемещаться между ветками.

### Слияние веток

* *git merge + name* - команда, которая осуществляет слияние текущей ветки с указанной.

_*NB*_ перед слиянием веток необходимо убедиться в том, что базовая и принимаемая ветки указаны верно!

### Типы слияния веток

* *слияние с конфликтом* - слияние, при котором изменения в ветках претендуют на одну и ту же область.

* *fast-forward* - слияние, при котором изменение происходило только в одной ветке. "Одна ветка опережает другую"

* *слияние через ort* - слияние, при котором в каждой ветке происходит свое уникальное изменение, не противоречащее друг другу.

### Удаление веток

_*NB*_ удаление веток не рекомендуется, поскольку будет нарушен порядок просмотра/изменений в репозитории/файле.

* *git branche -d + name* - команда, которая позволяет удалить ненужную ветку.

### Конфликты разрешаются с помощью команд:

* *git status* - команда, которая помогает идентифицировать конфликтующие во время слияния файлы.

* *git log --meige* - команда, которая создает журнал со списком конфликтов коммитов между ветками, для которых выполняется слияние.

* *git reset* - команда, которую можно использовать для разрешения конфликтов, возникающих во время выполнения слияния, чтобы восстановить заведомо удовлетворительное состояние конфликтующих файлов.

* *git meige --abort* - команда, при которой процесс слияния будет прерван, а ветка вернется к состоянию, в котором она находилась до начала слияния.

