# Алгоритм подбора соперника

У нас в photograd есть функция игры со случайным соперником. При этом создается игра, в которой второго игрока еще нет, либо игрок сам становится вторым игроком в игре. Вам необходимо реализовать алгоритм подбора соперников.

### Что влияет на подбор?

* Время ожидания - время, прошедшее с момента создания игры
* Рейтинг игроков - чем больше разница в рейтинге, тем меньше вероятности у игроков сыграть между собой
* Количество сыгранных игр - опытные пользователи больше играют с другими опытными пользователями, новички - больше с другими новичками
* Соперники в последних играх - не должно быть ситуации, когда 2 человека случайно выпадают друг на друга 5 раз подряд

### User

* id
* rating

### Game

* player1_id
* player2_id
* date_created