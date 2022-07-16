# Инструкция по работе с git

## что такое git?
Git — это набор консольных утилит, которые отслеживают и фиксируют изменения в файлах (чаще всего речь идет об исходном коде программ, но вы можете использовать его для любых файлов на ваш вкус). Изначально Git был создан Линусом Торвальдсом при разработке ядра Linux. Однако инструмент так понравился разработчикам, что в последствии, он получил широкое распространение и его стали использовать в других проектах. С его помощью вы можете сравнивать, анализировать, редактировать, сливать изменения и возвращаться назад к последнему сохранению. Этот процесс называется контролем версий.
## Подготовка репозитория

## Создание сохранений

## Журнал изменений

## Перемещение между "коммитами"
Для того, чтобы перемещатся между коммитами необходимо использовать команду "git checkout" для этого в терминале с папкой репозитория необходимо написать "git checkout <номер коммита>". Номер коммита берется из истории изменений. После такого перемещения мы попадаем в состояние **Detacher head**. Для возвращения в обычное состояние используется команда "git checout master".

## Ветки в git

## Слияние веток и решение конфликтов

## Удаление веток