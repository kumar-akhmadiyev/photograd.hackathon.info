# Frontend/Mobile

## Описание задания:

Необходимо написать мобильное приложение на iOS или Android, либо одностраничное веб приложение, отображающее статистику по вопросам, предложениям и миссиям партнера Photograd. Для получения данных Вам предстоит делать запросы на сервер photograd.

В конце страницы приведен список функций API, доступных для использования, а также описание формата используемых в них типов данных. На каждой странице указан метод запроса(GET или POST), URI этой функции, описание входных, выходных данных и возможных кодов ошибок. Значения в POST запросах передаются в виде JSON.

Ответы на запросы представлены в виде JSON с двумя полями - status и data. 
Значение поля status может быть success(запрос выполнен удачно), fail(произошла предвиденная ошибка) и error(непредвиденная ошибка). Поле data представляет собой JSON объект с данными, возвращаемыми функцией(формат данных описан на страницах функций). 

В первую очередь, Вам необходимо авторизоваться с помощью функции [логина](./UserLogin.md). Это необходимо для получения токена, который даст Вам доступ к другим функциям. Подробнее на странице с описанием функции.

С помощью GET запросов можно получить списки [вопросов](./GetQuestions.md), [предложений](./GetOffers.md) и [миссий](./GetMissions.md).
Затем, используя id объектов, можно получать по ним [статистику вопроса](./GetQuestionStatistics.md), [список покупок предложения](./GetOfferPurchases.md), [рейтинг миссии](./GetMissionRating.md) и [список наград миссии](./GetMissionRewards.md)

Адрес сервера : http://photograd.kz


#### Список функций API

* [User Login](./UserLogin.md)
* [Get questions](./GetQuestions.md)
* [Get question statistics](./GetQuestionStatistics.md)
* [Get offers](./GetOffers.md)
* [Get offer purchases](./GetOfferPurchases.md)
* [Get missions](./GetMissions.md)
* [Get mission rating](./GetMissionRating.md)
* [Get mission rewards](./GetMissionRewards.md)

#### Список объектов
* [Mission](./Mission.md)
* [AnswerOption](./AnswerOption.md)
* [Question](./Question.md)
* [Offer](./Offer.md)
* [Purchase](./Purchase.md)