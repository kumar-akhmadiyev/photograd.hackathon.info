# Get offer purchases
#### METHOD: POST 
#### URI: /hackathon/purchases

Получить список покупок предложения

#### Входные данные

    "offer_id" : integer

#### Выходные данные
    
    "purchases" : [<Purchase>]

#### Возможные ошибки

Код ошибки                      |    Описание
--------------------------------|--------------------------------
offer_not_exist                 | Данного предложения не существует
access_denied					| Отказано в доступе

#### Используемые объекты

* [Purchase](./Purchase.md)