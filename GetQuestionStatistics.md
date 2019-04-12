# Get question statistics
#### METHOD: POST 
#### URI: /hackathon/question_statistics

Получить статистику вопроса с id == question_id. Есть возможность ограничить временные рамки от from_date до to_date. Даты задаются строками вида "%d/%m/%Y %H:%M". Например - "13/04/2019 16:30"

#### Входные данные

    "question_id" : integer
    "date_from" : string  
    "date_until" : string

#### Выходные данные
    
    "views" : integer   // Общее количество просмотров
    "right_answers_percentage" : integer   // Процент правильных ответов
    "unique_users" : integer
    "by_sequence_number" : {              // Статистика показов в разрезе очередности
    	1 : {                             // Для показов вопроса в первый раз
            "views" : integer,
            "right_answers_percentage" : integer
        },
        2 : {                             // Для показов вопроса во второй раз
            "views" : integer,
            "right_answers_percentage" : integer
        }
        ......... и т.д.
    },
    "by_answer_options" : {               // В этом dictionary ключ - это id варианта ответа, а значение - процент ответов которые приходятся на этот вариант 
        (answer_option1_id : integer) : (percentage:integer)        
        (answer_option2_id : integer) : (percentage:integer)        
        (answer_option3_id : integer) : (percentage:integer)
        (answer_option4_id : integer) : (percentage:integer)
        -1 : (percentage:integer)                               // Варианты, в которых пользователь не выбрал ни один вариант ответа
    }


#### Возможные ошибки

Код ошибки                      |    Описание
--------------------------------|--------------------------------
wrong_date_format               | Некорретный формат даты
question_not_exist              | Данного вопроса не существует
access_denied                   | Отказано в доступе