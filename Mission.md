# Mission

### Поля

Название |   Тип                        | Описание         
---------|------------------------------|------------------
id       | integer                      |Идентификатор
title    | string						|Описание награды за миссию
description | string					|Описание миссии
company_name | string					|Название компании
status 	 | integer						|Статус миссии
notice   | string						|Примечания
due_date | string(datetime in isoformat)|Время окончания миссии
receive_instructions | string			|Инструкции по получению награды
games_played | integer					|Количество сыгранных игр
users_played | integer					|Количество участвовавших пользователей

### Статусы миссий

Название | Значение | Описание
---------|----------|----------
ACTIVE  | 1 | Активная миссия
FINISHED  | 3 | Завершенная миссия