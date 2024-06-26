# Прогнозирование оттока клиентов

## Описание проекта 

Из «Бета-Банка» каждый месяц понемногу стали уходить клиенты. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.

Нам предоставлены исторические данные о поведении клиентов и расторжении договоров с банком. 

От нас требуется проанализировать данные о клиентах «Бета-Банка» и построить ML-модель, прогнозирующую, уйдёт клиент из банка в ближайшее время или нет, со значением метрики *F1-мера* не менее *0.59.* 

## Используемые инструменты:
 
*Библиотеки:*
- pandas
- sklearn
- matplotlib
- numpy
 
## Результаты: 

- Мы загрузили и изучили данные, разбили на выборки, исследовали баланс классов и качество разных моделей и проверили модели на тестовой выборке.
  
- **Лучшие** показатели **F1-меры (0.6588235294117648)** и **'AUC-ROC' (0.8704296539423148)** получились у модели **"Случайный лес"** с количеством **деревьев: 30**, максимальной **глубиной: 7**, **критерием: "gini"**,  **random_state: 12345** и взвешиванием классов. Удалось избежать переобучения всех моделей.
