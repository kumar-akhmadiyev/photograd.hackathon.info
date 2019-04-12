# Frontend/Mobile

## Описание задания:

Необходимо написать мобильное приложение на iOS или Android, либо одностраничное веб приложение, отображающее статистику по вопросам, предложениям и миссиям партнера Photograd.
Для получения данных Вам предстоит делать запросы на сервер photograd.
В первую очередь, Вам необходимо авторизоваться с помощью функции [логина](./UserLogin.md). Это необходимо для получения токена, который даст Вам доступ к другим функциям. Подробнее на странице с описанием функции.

Адрес сервера : https://photograd.kz

sessionid, полученный при логине необходимо записывать в хидер X-SESSION-ID


#### Список функций API

* [User login](./UserLogin.md)
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