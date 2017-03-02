# redistest
Test example for use Redis on PHP to realise strong report as a WEB application.
### Аннотация
В статье рассмотрена возможность использования Redis для промежуточного хранения данных при реализации отчетов, требующих обработки больших массивов информации, как WEB приложений на PHP. На тестовом примере рассматриваются различные способы загрузки и обработки данных. Дается сравнение с реализацией аналогичного тестового примера на Oracle. 
## Описание
### Суть задачи
[Redis](https://cloud.github.com/downloads/kondratovich/the-little-redis-book/redis-ru.pdf) позиционируется как не реляционная СУБД, хранящая данные в оперативной памяти. Её применение эффективно, когда важна скорость обработки, например, для обеспечения быстрого доступа к очень загруженным WEB ресурсам. Подобная проблема возникает также [BI](https://ru.wikipedia.org/wiki/Business_Intelligence) (Business Intelligence) инструментах,  в задачах промежуточной обработки в [ETL](https://ru.wikipedia.org/wiki/ETL)(Extract, Transform, Load) системах. Например, в [QlikView](http://www.qlik.com/ru-ru/company)  обработка данных реализована тоже в оперативной памяти.
В связи с этим представляется интересным посмотреть, насколько можно приспособить Redis к решению задач ETL и BI.
### Описание тестового примера
![Схема таблиц тестового примера](https://github.com/sergechurkin/redisaggregate/blob/master/redisaggregate.png)
### Методика тестирования и ее реализующая программа  
Тестирование проводилось на компьютере с процессором 2.2ГГц, ОЗУ 4Гб, ОС Win7x64. [XAMPP](https://www.apachefriends.org/download.html) 7.0.9. Redis_version:3.2.100. 
### Как лучше и быстрее загружать данные?
### Сравнение результатов
### Выводы
## Установка
    composer create-project sergechurkin/
Параметры настройки и подключения к серверу Redis задаются в `params.php`.

