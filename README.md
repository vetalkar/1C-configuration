# 1C-configuration

###Возможности

* Обмен заказами
* Выгрузка каталога
* Выгрузка цен и остатков


###Объекты интеграции

* Общий модуль - Интаро_общий
* Подписка на событие - Интаро_документы
* Константа - Интаро_константы
* Обработка - IntaroШаблонноеРешение

###Порядок интеграции

* Добавляем объекты в конфигурацию
* С помощью обработки инициализируем константы, сохраняем.
* С помощью обработки выполняется загрузка заказов из ЦРМ, выгрузка остатков и цен в retailCRM, и если есть необходимость то и выгрузка каталога номенклатуры в ЦРМ.
* Выгрузка данных по заказу из 1С в ЦРМ происходит при проведении заказа.
* Для этих целей и нужна подписка на событие. Её настраиваем под нужную конфигурацию.