# Offer Restriction

### Поля

Название    |   Тип                        | Описание         
------------|------------------------------|------------------
id          | integer                      |Идентификатор     
restriction_type | integer				   |Тип ограничения(0-ограничение за все время,1-ограничение за период времени)
amount      | integer					   |Максимум
period      | integer 					   |Период ограничения. Поле возвращается только при restriction_type == 1

