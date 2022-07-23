Cоздадим виртуальное окружение (оно также называется `virtualenv`). `Virtualenv` будет изолировать настройки Python/Django для каждого отдельного проекта. 
Это значит, что изменения одного сайта не затронут другие сайты, которые ты разрабатываешь. Удобно, правда?

Всё, что тебе нужно сделать — найти директорию, в которой мы создадим `virtualenv`; домашний каталог вполне подойдёт. 
Для Windows адрес будет выглядеть так: `C:\Users\Name` (где `Name` — твоё имя пользователя).

>Примечание: Если ты работаешь в Windows, удостоверься, что в названии директории нет специальных символов или символов с диакритическими знаками; если в твоём имени пользователя есть такие символы, выбери другую директорию, например, `C:\djangogirls`.

Мы будем использовать отдельную директорию `djangogirls` в домашнем каталоге:

`command-line`
```
$ mkdir djangogirls
$ cd djangogirls
```
Мы создадим виртуальное окружение под именем `myvenv`. В общем случае команда будет выглядеть так:

`command-line`
```
$ python3 -m venv myvenv
```
## Виртуальное окружение: Windows

Чтобы создать новое `virtualenv`, тебе нужно открыть командную строку и набрать `python -m venv myvenv`. Это будет выглядеть так:

`command-line`
```
C:\Users\Name\djangogirls> python -m venv myvenv
```
Здесь `myvenv` — имя твоего `virtualenv`. Ты можешь выбрать другое имя, но используй только строчные буквы, без пробелов и специальных символов. *Имя виртуального окружения выбирай покороче — тебе придётся часто его набирать!*

## Работаем с virtualenv
Указанная выше команда создаст директорию myvenv (или другую, в зависимости от выбранного тобой имени), которая будет содержать виртуальное окружение (по сути — набор файлов и папок).

Запусти виртуальное окружение, выполнив:

`command-line`
```
C:\Users\Name\djangogirls> myvenv\Scripts\activate
```
>**Примечание:**  в Windows 10 при работе в Windows PowerShell ты можешь получить ошибку вида `execution of scripts is disabled on this system`. В этом случае открой ещё одно окно Windows PowerShell, выбрав опцию «Запустить от имени Администратора». Затем перед использованием виртуального окружения попробуй запустить следующую команду:
`command-line`
```
C:\WINDOWS\system32> Set-ExecutionPolicy -ExecutionPolicy RemoteSigned
    Execution Policy Change
    The execution policy helps protect you from scripts that you do not trust. Changing the execution policy might expose you to the security risks described in the about_Execution_Policies help topic at http://go.microsoft.com/fwlink/?LinkID=135170. Do you want to change the execution policy? [Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"): A
```
