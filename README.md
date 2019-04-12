# Описание API для хакатона Photograd

Адрес сервера : photograd.kz

sessionid, полученный при логине необходимо записывать в хидер X-SESSION-ID


#### Список функций API

* Questions
	* [Get question](./GetQuestion)
    * [Get questions](./GetQuestions)
    * [Get question statistics](./GetQuestionStatistics)
* Categories
	* [Get category](./GetCategory)
	* [Get categories](./GetCategories)
* Offers
	* [Get offers](./GetOffers)
	* [Get offer purchases](./GetOfferPurchases)
* Missions
	* [Get missions](./GetMissions)
	* [Get mission rating](./GetMissionRating)
	* [Get mission rewards](./GetMissionRewards)

#### Список объектов
* [User](./User)
* [Game](./Game)
* [Image](./Image)
* [Friend](./Friend)
* [Mission](./Mission)
* [Mission attempt](./MissionAttempt)
* [Achievement](./Achievement)
* [AchievementProgress](./AchievementProgress)
* [Gameround](./Gameround)
* [Answer](./Answer)
* [AnswerOption](./AnswerOption)
* [Question](./question.md)
* [QuestionInstance](./QuestionInstance)
* [Category](./Category)
* [Notification](./Notification)
* [Offer](./Offer)
* [Purchase](./Purchase)
