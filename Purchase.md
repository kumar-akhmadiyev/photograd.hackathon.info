# Purchase

### Поля

Название    |   Тип                        | Описание         
------------|------------------------------|------------------
id          | integer                      |Идентификатор     
username     | string                      |Имя пользователя, совершившего покупку
purchase_date   | string(date in isoformat)    |Дата совершения покупки
activation_date| string(date in isoformat) |Дата активации покупки(В случае, если status = ACTIVATED)
expiration_date| string(date in isoformat) |Дата активации покупки(В случае, если status = NOT_ACTIVATED,EXPIRED)
status 		| integer					   |Статус покупки
unique_code | string                       |Уникальный код покупки

### Статусы покупок

Название | Значение | Описание
---------|----------|----------
NOT_ACTIVATED  | 0 | Не активирована
ACTIVATED  | 1 | Активирована
EXPIRED	 | 2  | Истек срок годности