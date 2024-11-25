# Исследование надежности заемщиков

## Описание проекта 

Заказчик — кредитный отдел банка. Нам нужно разобраться, **влияет ли семейное положение и количество детей клиента на факт погашения кредита в срок.** Входные данные от банка — статистика о платёжеспособности клиентов.

Результаты исследования будут учтены при построении модели кредитного скоринга — специальной системы, которая оценивает способность потенциального заёмщика вернуть кредит банку.


## Используемые инструменты:
 
*Библиотеки:*
- pandas
 
## Результаты: 

- Мы загрузили таблицу и ознакомились с данными, провели предобработку, исследовали данные и проверили гипотезы.

- **Семейное положение и количество детей** клиента **влияют на факт погашения кредита в срок**, но это влияние не линейно: у клиентов, имеющих пять детей, просрочки отсутствовали, а у имеющих четверых детей, просрочка наивысшая (9,76%).

- В целом, **клиенты с детьми чаще допускали просрочку**. 

- В то же время, **неженатые/незамужние** имели **наибольший показатель** невозврата кредита в срок **(9,76%)**, среди **вдовцов/вдов** этот показатель **наименьший (7,06%)**.

- В целом, **заемщики, состоящие или состоявшие в браке, реже допускали просрочку.** 
