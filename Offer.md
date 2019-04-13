# Offer

### Поля

Название    |   Тип                        | Описание         
------------|------------------------------|------------------
id          | integer                      |Идентификатор     
title 		| string 					   |Название предложения
description | string					   |Описание предложения
after_activation_text | string	  		   |Текст после активации предложения 
receive_instructions | string			   |Инструкции по получению
notice 		| string		               |Замечания
price 		| integer 						| Цена      			
initial_amount 	| integer 					| Начальное количество
current_amount 	| integer 					| Текущиее количество
deposit 		| string  					| Минимальный депозит
restrictions | [<OfferRestriction>]  			| Ограничения предложений
image | string								| Ссылка на предложение

#### Используемые объекты

* [OfferRestriction](./OfferRestriction.md)