# Инструкция по работе с git
## что такое git?
Git — это набор консольных утилит, которые отслеживают и фиксируют изменения в файлах (чаще всего речь идет об исходном коде программ, но вы можете использовать его для любых файлов на ваш вкус). Изначально Git был создан Линусом Торвальдсом при разработке ядра Linux. Однако инструмент так понравился разработчикам, что в последствии, он получил широкое распространение и его стали использовать в других проектах. С его помощью вы можете сравнивать, анализировать, редактировать, сливать изменения и возвращаться назад к последнему сохранению. Этот процесс называется контролем версий.
## Подготовка репозитория
для создания репозитория используется команда "git init". В терминале в папке с будущим репозиторием достаточно написать "git init", и эта папка станет репозиторием.
Это первое, что нужно сделать для нового проекта.
git config --global user.name "Ваше Имя"
git config --global user.email "ВашаПочта@mail.com"
Эти случаи отмечаются при каждой фиксации (исправлении изменений) в Республике . Их установка стоит всего один раз при установке Git.
## Создание коммитов
git commit -m "Описание коммита"
Берёт файлы из промежуточной области и «фиксирует» их в Вашем локальном репозитории. В кавычки следует вставить краткое описание изменений для ряда коммитов. Постарайтесь описать коммит с краткими деталями, например: «устранил проблему при использовании имени пользователя» вместо создания «каких-то изменений».
### Добавление файла в коммит
Для добавления файла в текущий коммит используется команда "git add". Для этого достаточно в терминале с папкой текущего репозитория написать "git add <название файла>".
### Сохранение коммита
Для сохранения коммита используется команда "git commit". Для этого в терминале с папкой репозитория необходимо написать команду "git commit -m <сообщение к коммиту>". Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.
Команда "git status" выводит список проиндексированных и неотслеживаемых файлов, а также файлов, удаленных из индекса Git. Команда git status относительно проста в использовании. Она показывает, какие изменения были внесены с помощью команд git add и git commit. Сообщения о состоянии также содержат инструкции по индексированию файлов либо отмене этой операции.
## Журнал изменений
Для посмотра историй коммитов, то есть истории наших изменений используется команда "git log". Для этого необходимо в терминале с папкой-репозиторием написать "git log".
## Перемещение между "коммитами"
Для того, чтобы перемещатся между коммитами необходимо использовать команду "git checkout" для этого в терминале с папкой репозитория необходимо написать "git checkout <номер коммита>". Номер коммита берется из истории изменений. После такого перемещения мы попадаем в состояние **Detacher head**. Для возвращения в обычное состояние используется команда "git checout master".
## Ветки в git
Создайте ветвь на основе кода в текущей ветви, например mainпри запуске новой работы. Рекомендуется проверить, какая ветвь выбрана git status перед созданием новой ветви.
Создайте ветви в Git с помощью git branch команды:
"git branch <branchname>"
## Слияние веток и решение конфликтов
Для слияние веток используются следующие команды:
- "git branch <названиеВетки>"
Создает сущность, определяемую ветвь (ветвь) . Ветвь - это точная копия Ваших файлов.
- "git checkout <названиеВетки>”
Разрешите Вам переключить контроль над созданной вами веткой и работать в ее пределах. Здесь Вы можете производить любые изменения кода. Когда вы будете разрабатывать, можно будет зафиксировать изменения или же можно удалить ветвь, если ниже что-то пошло не так или Вам больше не нужны изменения, сделанные в этой ветке.
## Удаление веток
Команда для удаления локальной ветки в Git:
"git branch -d  <название ветки>", где
-d – флаг, опция команды git branch, сокращенный вариант записи --delete. Как и следует из названия, предназначен для удаления ветки.
## Получение удалённого репозитория
Для того, чтобы скачать удалённый репозиторий необходимо использовать команду git clone. В терминале, в котором открыта любая пустая папка, необходимо написать git clone <ссылка на репозиторий>. Репозиторий скачатеся в папку, название которой будет совпадать с названием репозитория.
