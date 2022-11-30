# Инструкция для работы с Markdown
## Заголовки

# Инструкция для работы с Markdown
## Инструкция для работы с Markdown
### Инструкция для работы с Markdown
#### Инструкция для работы с Markdown
##### Инструкция для работы с Markdown

Чем больше количество (#) тем меньше размером будет заголовок.

## Содержание

Чтобы сделать содержание с тегом на содержимое в тексте 
можно воспользоваться вот такой формой:

[Описание](#название абзаца).

1. [Выделение текст](#выделение-текста)
2. [Списки](#списки)
3. [Работа с изображениями](#работа-с-изображениями)
4. [Ссылки](#ссылки)
5. [Работа с таблицами](#работа-с-таблицами)
6. [Цитаты](#цитаты)
7. [Заключение](#заключение)




# Выделение текста 
Чтобы выделить текст курсивом необходимо обрамить его звездочками (*) или (_).Например , *вот так* или _вот так_.

Чтобы выделить текст полужирным,необходимо обрамить его двойными звездочками (**) или (__) Например, **Вот так** или __Вот так__.

Альтернативные способы выделения текста полужирным или курсивом нужны для того что бы мы могли совмешать оба этих способа. 
Например, _текст может выделен курсивом_ и при этом быть **полужирным**.

Две тильды перечёркивают текст. ~~Перечеркнутый текст~~

## Списки

Чтобы добавить ненумерованный списки, необходимо пункты выделить звездочкой (* ).
Например, вот так:
* Элемент1
* Элемент2
* Элемент3

Что добавить пронумерованные списки, необходимо их пронумеровать (1. ).
Например, вот так:
1. Первый пункт
2. Второй пункт
3. Третий пункт

## Работа с изображениями

Чтобы вставить изображения, достаточно написать следующее :
![Привет это image](image.png)


## Ссылки

Для того чтобы вставить ссылку достаточно написать следующее:
![Ссылка!](URl aдрес "Комментарий если нужно")

Например, вот так : 
![Сcылка!](https://ru.markdown.net.br/bazovyy-sintaksis/#table-1-5/"Синтаксис языка Markdown")

Так же любая ссылка обрамленная угловыми скобками (<>) преобразуется в ссылку.

Например : <https://ru.markdown.net.br/bazovyy-sintaksis/#table-1-5/>

## Работа с таблицами

| Tables | Are | Cool |
|---------------|:--------------:|--------------:|
|cool 3 is      | rigth-aligned  | 1600$         |
|cool 2 is      | centered       | 12$           |
|zebra stripes  | are neat       | 1$            |

Обязательно требуют заголовок и настройки выравнивания (второй строкой). Выравнивание задаётся двоеточием. Колонки задаются вертикальным палками (|)

Markdown | Less | Pretty
----|----|-----|
*still* | `renders` | **nicely** 
1 | 2 | 3

Внешние вертикальные палки (|) задавать необязательно, также не требуется подгонять колонки под один размер. Можно использовать стили, описанные выше.

## Цитаты

> Цитаты задаются угловой скобкой.
> Это строка является частью цитаты.

Здесь цитата прерывается.

>Можно писать много-много текста, и он автоматически всё преобразует в одну цитату. Также можно использовать разилчные *начертания* в **цитате**.
  
## Работа с удаленным репозиторием

Удалённые репозитории представляют собой версии вашего проекта, сохранённые в интернете или ещё где-то в сети. У вас может быть несколько удалённых репозиториев, каждый из которых может быть доступен для чтения или для чтения-записи. Взаимодействие с другими пользователями предполагает управление удалёнными репозиториями, а также отправку и получение данных из них. Управление репозиториями включает в себя как умение добавлять новые, так и умение удалять устаревшие репозитории, а также умение управлять различными удалёнными ветками, объявлять их отслеживаемыми или нет и так далее.

Для того что бы добавить удаленный репозиторий и присвоить ему имя нужно использовать команду:

git remote add (shortname) (url)

Для того что бы добавить копию удаленного репозитория к себе  нужно использовать команду:

git clone (url) адрес удаленного репозитория

Далее убедится в том, что вы находитесь в папке добавленного репозитория и если нужно перейти в него командой:

cd (название репозитория)

Для того, чтобы просмотреть список настроенных удалённых репозиториев, вы можете запустить команду  git remote.

 Она выведет названия доступных удалённых репозиториев. Если вы клонировали репозиторий, то увидите как минимум origin — имя по умолчанию, которое Git даёт серверу, с которого производилось клонирование.

Вы можете также указать ключ -v (git remote -v), чтобы просмотреть адреса для чтения и записи, привязанные к репозиторию.

Так же вы можете посмотреть все commit данного репозитория используя команду:

git log --oneline --all --graph

После того как вы закончили работу с данным репозиторием и зафиксировали все изменения. Вы можете отправить эту версию с измененными данными на GitHub  для дальнейшего pull&request используя команду:

git push

Что бы вытащить информацию из удаленного репозитория к себе  вы можете воспользоваться командой:

git pull 

Что бы ваша измененная версия дошла до основного источника репозитория вам нужно после команды git push , перейти на GitHub и создать pull&request написать если нужно комментарий и отправить. Позже создатель репозитория увидит вашу изменную версию репозитория и примет решение что от туда взять или убрать, либо вернет на доработку с комментарием.

## Заключение
 В данной инструкции описывается использование работы с языком Markdown и Git так называемая шпаргалка.