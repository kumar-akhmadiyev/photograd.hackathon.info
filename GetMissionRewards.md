# Get mission rewards
#### METHOD: GET 
#### URI: /hackathon/mission_rewards

Получить список наград за миссию. Метод предназначен только для завершенных миссий, то есть тех, у которых status == 3

#### Входные данные

    "mission_id" : integer

#### Выходные данные
    
    "rewards" : [<MissionReward>]

#### Возможные ошибки

Код ошибки                      |    Описание
--------------------------------|--------------------------------
partner_mission_not_exist                  | Данной миссии не существует

#### Используемые объекты

* [MissionReward](./MissionReward.md)