Легенда

Заказчик передал вам файл в формате Excel, в котором сформирован отчёт.

На основе этого отчёта нужно выполнить следующие задания.

Задание 1
Опишите не менее семи таблиц, из которых состоит база данных:

какие данные хранятся в этих таблицах;
какой тип данных у столбцов в этих таблицах, если данные хранятся в PostgreSQL.
Приведите решение к следующему виду:

Сотрудники (

идентификатор, первичный ключ, serial,
фамилия varchar(50),
...
идентификатор структурного подразделения, внешний ключ, integer).


Ответ.

Сотрудники

Идентификатор (первичный ключ serial),

Фамилия, Имя, Отчество, varchar(100),

Дата приема на работу (Date),

Оклад (DECIMAL 10, 2), оклад_id (INTEGER),

Должность, varchar(100), должность_id (INTEGER),

Тип подразделения, VARCHAR(50), код_подразделения_id (INTEGER),

Структурное подразделение, VARCHAR(50), код_структурного_поразделения_id (INTEGER),

Филиал, VARCHAR(50), название_города_id (INTEGER),

проект, VARCHAR(50), проект_id (INTEGER)

Должность

Идентификатор (первичный ключ serial),

Должность, varchar(100)

Идентификатор_сотрудника_id (INTEGER)

Тип подразделения

Идентификатор (первичный ключ serial),

Тип подразделения (полное название), varchar(100)

Идентификатор_структурного_подразделения_id (INTEGER)

Код структурного поразделения

Идентификатор (первичный ключ serial),

Полное наименование структурного подразделения, varchar(100)

Идентификатор_должности_id (INTEGER)

Филиал

Идентификатор (первичный ключ serial),

Полный адрес филиала, varchar(255)

Проект

Идентификатор (первичный ключ serial),

Наазвание проекта, varchar(100)

Идентификатор_сотрудника_id (INTEGER)

Назначение на проект

Идентификатор_проекта_id (INTEGER)

Идентификатор_сотрудника_id (INTEGER)

Оклад

Идентификатор (первичный ключ serial),

Идентификатор_должности_id (INTEGER)

Идентификатор_сотрудника_id (INTEGER)
