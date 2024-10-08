# Телеком. Прогнозирование оттока клиентов
## Описание проекта

- Оператор связи «ТелеДом» борется с оттоком клиентов. Для этого его сотрудники будут предлагать промокоды и специальные условия всем, кто планирует отказаться от услуг связи. Чтобы заранее находить таких пользователей, «ТелеДому» нужна модель, которая будет предсказывать, разорвёт ли абонент договор.

## Цель

- На предоставленных оператором данных необходимо обучить модель прогнозировать отток клиентов со значением метрики ROC-AUC на тестовой выборке не менее 0.85.

## Используемые инструменты:
 
*Библиотеки:*
 
-   pandas
-	numpy
-	matplotlib
-	sklearn
-   phik
-   sqlalchemy
-   catboost
-   lightgbm

*Модели:*

-	DummyClassifier. 
-	LogisticRegression.
-	RandomForestClassifier.
-   LGBMClassifier.
-	CatBoostRegressor.
-	MLPClassifier.

## Результаты: 

-  Мы подключились к базе и загрузили таблицы sql, исследовали и подготовили данные для обучения.

-  На подготовленных данных мы обучили разные модели, попробовав для каждой разные гиперпараметры и отобрали модель с лучшей метрикой ROC_AUC на кросс-валидации. Затем, мы протестировали лучшую модель и продемонстрировали её работу.

-  Лучшая модель *CatBoostClassifier* показала значение **ROC_AUC тестовой выборки – 0.858437**. Что выше заявленной цели. 

-  Мы предложили лучшую модель заказчику и дали свои рекомендации по ее использованию и повышению качества и точности прогноза.
