# Mission Reward

### Поля

Название 	|   Тип                        | Описание         
------------|------------------------------|------------------
id       	| integer                      |Идентификатор     
username    | string			           |Имя пользователя
place		| integer					   |Занятое место
last_victory_date| string(datetime in isoformat)   |Дата последней победы
unique_code | string					   |Уникальный код награды
status		| integer					   |Статус награды
games_played| integer					   |Количество сыгранных игр
victories   | integer					   |Количество побед					

### Статусы наград

Название | Значение | Описание
---------|----------|----------
NOT_ACTIVATED  | 1 | Не активирована
ACTIVATED  | 2 | Активирована