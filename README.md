# simpleshop

https://drive.google.com/drive/folders/1u9KvXf3d_AWiXopaQTMxW55C3cs8IMy3?usp=sharing ( есит больше порогового размера для гита, поэтому загрузил на Диск)

Задание: написать любой сайт на фреймворке  php Laravel и подключить к нему БД, написанную по модели  EAV. Был написан простой интернет-магазин с базовым функционалом, который использует встраиваемую СУБД Sqlite. В БД присутствуют 3 изначальные таблицы 


shop_orders, shop_products, shop_categories. На основе этих не связанных между собой таблиц были созданы таблицы по модели EAV: shop_attribute_all(хранит в себе все параметры, которые относятся к предыдщим трем таблицам), shop_entity_type(таблица хранит id всё тех же трёх таблиц) и 3 таблицы значений shop_value_client, shop_value_datetime, shop_value_meta(хранят в себе значения всех полей через  id  сущностей и id наших параметров). БД можно открыть через DB browser(apt-get install sqlitebrowser).

