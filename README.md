# simpleshop

https://drive.google.com/drive/folders/1u9KvXf3d_AWiXopaQTMxW55C3cs8IMy3?usp=sharing (проект(архив) весит больше порогового размера для гита, поэтому пришлось загрузить на гДиск)

Задание: написать любой сайт на фреймворке  php Laravel и подключить к нему БД, написанную по модели  EAV.

Был написан простой интернет-магазин с базовым функционалом, который использует встраиваемую СУБД Sqlite. В БД присутствуют 3 изначальные таблицы shop_orders, shop_products, shop_categories. На основе этих не связанных между собой таблиц были созданы таблицы по модели EAV: shop_attribute_all(хранит в себе все параметры, которые относятся к предыдщим трем таблицам), shop_entity_type(таблица хранит id всё тех же трёх таблиц) и 3 таблицы значений shop_value_client, shop_value_datetime, shop_value_meta(хранят в себе значения всех полей через  id  сущностей и id наших параметров). БД можно открыть через DB browser(apt-get install sqlitebrowser). Таблицы по модели EAV не привязаны к коду сайта, но зато к ним подвязаны классические таблицы, которые вложены в бд. Основной плюс модели EAV заключается в том, что мы имеем доступ к легкому добавлению доп параметров к нашей бд. Данный подход несколько снижает скорость работы базы данных, но при этом облегчает работу с ней.

Скрины сайта находятся по той же ссылке.
