# Get mission rating
#### METHOD: GET 
#### URI: /hackathon/mission_rating

Получить рейтинг партнерской миссии. Метод предназначен только для активных миссий, то есть тех, у которых status == 1

#### Входные данные

    "mission_id" : integer

#### Выходные данные
    
    "rating" : [{
    	'place': integer,
    	'username' : string,
    	'games_played': integer,
    	'victories' : integer
    }]     

#### Возможные ошибки

Код ошибки                      |    Описание
--------------------------------|--------------------------------
mission_not_exist				| Такой миссии не существует
wrong_mission_status			| Некорректный статус миссии