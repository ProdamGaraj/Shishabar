# Project Shishabar

## PureBackend

1. Хранение чеков

2. Курс валют с цб 

3. Система лояльности:
   - Система скидок и лояльности (скидки фиксированые, одинаковые меняются по времени)
   - Выяснить про их карточки!
   - Отслеживание одного и того же пользователя 
     - Первой скидки нет, если нет номера телефона
     - Для юзера сделать JWT токен на неделю-месяц

4. Оплата (Click)

5. Табло для вывода пинкода в зал (id вшиты в куар и отвечают исключительно за стол)

***Идея:***
    `кастомные блюда ,чай.`

## Клиент

1. Регистрация по номеру телефона (подтверждение смс)

2. Подтверждение что в зале?

3. Просмотр меню

4. Заказ корзины из позиций меню (кальяны тоже в меню)

5. Проверка на наличие перед оплатой

***Идея:***
    `доставка`


## Бэкофис

Все регаются, глав админа добавляем сами. У всех соотвественно изменение (востановление) пароля

### Офики и стафф (1 устройство)
1. Смена пароля раз в смену

2. Подтверждение возраста сотрудником (значок ожидания у клиента до момента подтверждения сотрудником)

3. Заканчивающиеся ингридиенты менеджер вводит вручную, что вызывает эффект "не в наличии" у элемента меню с этим ингридиентом

4. Наполнение меню

***Идея:***
    `подумать над регистраией официантов в системе (не под авторизацию) для сохранения статистики по кол - ву вынесенных заказов.
Как сделать? При попадании заказа в бэкофис свободный официант выбирает заказ, нажмает на кнопочку со своим Фамилия И.О. далее тречит этот заказ(оплачен = готовится, ожидает выдачи, выдан, завершён)`


### Гендир 

Вывод статистики по:
- кол-во заказов
- сумма заказов за (смена/день/неделя/месяц) календарь имба

## Бот
    
1. Уведомления от бота о смене пароля для стаффа

2. Для брони мест

## Технологический стек:
- Java Spring `as` бэкенд 
- Gradle || Maven `as` система сборки
- JS React `as` фронтенд
- Docker `as` контейнеры
- Cheff || Puppet || Compose `as` оркестратор
- PostgreSQL + MongoDB || Redis `as` субд

# ALFA
## Поднять функционал куаркодов на том что есть

## Функцианал прости господи...

- Какие куары юзать????
- Просмотр меню (если не в наличии то показывать плашку)
- Карточка товара:
  - Фотка
  - Описание товара
  - Граммовка
  - Цена
  - Кнопка "в заказ\корзину" Если мин 1 такой в карзине показывать - n + (n-кол-во)
- Заказ корзины из позиций меню (кальяны тоже в меню)
- Проверка на наличие перед оплатой
- Чай - это 20% отображать отдельно.
- Оплата
- Чек показываем после оплаты, оставляем на клик\пейми
- Все чеки храним
- Ввод меню делаем мы (пока что)
- Интеграция с iiko

API????

- Оплата
  - Как зарегистрировать нас для оплаты
  - Есть ли запрос на оплату через iiko
    - Как работает оплата через iiko
    - Что происходит, если оплаты не происходит
  - Как в создании заказа указать стороннюю оплату
- Сервер
  - Обязательно ли на C#?
  -  