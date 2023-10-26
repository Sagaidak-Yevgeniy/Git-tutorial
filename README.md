# Git-tutorial
Подробная инструкция работы с GIT
# Инструкция по работе с GIT в CLI Интерфейс командной строки (англ. Command Line Interface, CLI)

## Устанавливаем необходимое программное обеспечение:

 - Скачиваем и устанавливаем [git](https://git-scm.com/downloads) 
 - Скачиваем и устанавливаем текстовый редактор [VisualStudioCode](https://code.visualstudio.com/) 

## Регистрация на необходимых сервисах:

 - Регистрация на [GitHUB](https://github.com/) 

## Пошаговая инструкция начала работы с технологией GIT : 


1. ### Инструкция работы с GIT локально:

     - Создаем папку со своим проектом или переносим файлы уже готового проекта (файлы .html .css .js папки и т.д.)
     - Запускаем VisualStudioCode
     - Нажимаем в верхнем меню `File`  `OpenFolder`   Указываем путь к папке которую создали ранее
     - Запускаем терминал в VisualStudioCode  `Terminal`  `New Terminal`
     - Команда `git init`    (Позволяет проинициализировать репозиторий в текущей папке)
     - Команда `git status`   (Показывает текущий статус)
     - Команда `git add`  (Отслеживает изменения файлов
`git add index.html` — добавляет index.html
`git add . ` — добавляет все файлы
)  
     - Команда `git config`  (Конфигурация и параметры git
`git config --global user.name` — Показывает имя пользователя
`git config --global user.name 'new user'` — Изменяет имя пользователя
`git config --global user.email` — Показывает email пользователя
`git config --global user.email 'test@mail.ru'` — Изменяет email пользователя
)
     - Команда `git commit -m 'commit message'`  (создает коммит с сообщением)
     - Команда `git log`  (Просмотр всех commit(для выхода из режима просмотра нажмите клавишу`Q`  ))  
     - Команда `git branch`  
(Работа с ветками в репозитории
`git branch` — показывает список веток
`git branch branch-name` — создает новую ветку branch-name
`git branch -D branch-name` — удаляет ветку branch-name)  
     - Команда `git checkout`  
(Переключается на другую ветку
`git checkout branch-name` — переключается на последний коммит в ветке branch-name
`git checkout -b branch-name` — создает и переключается на ветку branch-name)  
     - Команда `git merge` 
(Совмещает текущую ветку с выбранной
`git merge branch-name` — совмещает текущую ветку с branch-name)

     - Прописываем команду ` git checkout commit_id`  (Перейти к нужному коммиту, id можно посмотреть командой `git log`)  
     - Прописываем команду `git reset --hard commit_id`  (откатить до определенного коммита)  

2. ### Инструкция работы с GIT глобально с удаленным репозиторием GitHub:
#### Есть два варианта либо мы себе в репозиторий загружаем проект, либо в чужой репозиторий начнем если вам нужно загрузить в свой репозиторий:

-	Создаем репозиторий на GitHub: авторизуемся под своим логином паролем на портале  в правом верхнем углу нажимаем на иконку профиля  Выбираем из списка `Your repositories`  справа нажимаем на кнопку `New`  Вводим имя репозитория `Repository name`  Вводим небольшое описание репозитория `Description` Далее выбираем каким будет реппозиторий публичным `Public` или приватным `Private` после можно поставить галочки если вам нужен файл README `Add a README file` или файл .gitignore
`Add .gitignore`  Нажимаем на кнопку `Create Repository`
-	После откроется окно где будут показаны команды CLI, вам нужно использовать только две команды
-	Вводим в терминале команду находясь в своей папке с настроенным локально проектом с хотя бы минимум одним коммитом  `git remote add origin https://github.com/Имя вашегоаккаунта/Названиепроекта.git` ссылку можно скопировать в появившемся окне (см предыдущий пункт)
-	Вторая команда `git push -u origin branch-name`  (где branch-name имя вашей ветки, если вдруг что то пойдет не так сам гит подскажет какую команду ввести)
-	Если вы все сделали правильно то зайдите в браузер и обновите страницу создания репозитория













