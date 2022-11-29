# HW1_SQL

 **Вывести все поля и все строки.**
 ```SQL
select * from students;
 ```
 **Вывести только Id пользователей**
 ```SQL
select id from students;
 ```
 **Вывести только имя пользователей**
 ```SQL
select name from students;
 ```
 **Вывести только email пользователей**
 ```SQL
select email from students;
 ```
 **Вывести имя и email пользователей**
 ```SQL
select name, email from students;
 ```
 **Вывести id, имя, email и дату создания пользователей**
 ```SQL
select id, name, email, created_on from students;
 ```
 **Вывести пользователей где password 12333**
 ```SQL
select * from students where "password" = '12333';
 ```
 **Вывести пользователей которые были созданы 2021-03-26 00:00:00**
 ```SQL
select * from students where created_on  = '2021-03-26 00:00:00';
 ```
 **Вывести пользователей где в имени есть слово Анна**
 ```SQL
select name from students where name like '%Anna%';
 ```
 **Вывести пользователей где в имени в конце есть 8**
 ```SQL
select name from students where name like '%8';
 ```
 **Вывести пользователей где в имени в есть буква а**
 ```SQL
select name from students where name like '%a%';
 ```
 **Вывести пользователей которые были созданы 2021-07-12 00:00:00**
 ```SQL
select * from students where created_on = '2021-07-12 00:00:00';
 ```
 **Вывести пользователей которые были созданы 2021-07-12 00:00:00 и имеют пароль 1m313**
 ```SQL
select * from students where created_on = '2021-07-12 00:00:00' and "password" = '1m313';
 ```
 **Вывести пользователей которые были созданы 2021-07-12 00:00:00 и у которых в имени есть слово Andrey**
 ```SQL
select * from students where created_on = '2021-07-12 00:00:00' and name like '%Andrey%';
 ```
 **Вывести пользователей которые были созданы 2021-07-12 00:00:00 и у которых в имени есть цифра 8**
 ```SQL
select * from students where created_on = '2021-07-12 00:00:00' and name like '%8%';
 ```
 **Вывести пользователя у которых id равен 110**
 ```SQL
select * from students where id = '110';
 ```
 **Вывести пользователя у которых id равен 153**
 ```SQL
select * from students where id = 153;
 ```
 **Вывести пользователя у которых id больше 140**
 ```SQL
select * from students where id > 140 order by id;
 ```
 **Вывести пользователя у которых id меньше 130**
 ```SQL
select * from students where id < 130 order by id;
 ```
 **Вывести пользователя у которых id меньше 127 или больше 188**
 ```SQL
select * from students where id < 127 or id > 188;
 ```
 **Вывести пользователя у которых id меньше либо равно 137**
 ```SQL
select * from students where id <=137;
 ```
 **Вывести пользователя у которых id больше либо равно 137**
 ```SQL
select * from students where id >= 137;
 ```
 **Вывести пользователя у которых id больше 180 но меньше 190**
 ```SQL
select * from students where id > 180 and id < 190;
 ```
 **Вывести пользователя у которых id между 180 и 190**
 ```SQL
select * from students where id between 180 and 190;
 ```
 **Вывести пользователей где password равен 12333, 1m313, 123313**
 ```SQL
select * from students where "password" = '12333' or "password" = '1m313' or "password" = '123313';
 ```
 **Вывести пользователей где created_on равен 2020-10-03 00:00:00, 2021-05-19 00:00:00, 2021-03-26 00:00:00**
 ```SQL
select * from students where created_on = '2020-10-03 00:00:00' or created_on = '2021-05-19 00:00:00' or created_on = '2021-03-26 00:00:00';
 ```
 **Вывести минимальный id**
 ```SQL
select min(id) from students;
 ```
 **Вывести максимальный.**
 ```SQL
select max(id) from students;
 ```
 **Вывести количество пользователей**
 ```SQL
select count(*) from students;
 ```
 **Вывести id пользователя, имя, дату создания пользователя. Отсортировать по порядку возрастания даты добавления пользоватлеля.**
 ```SQL
select id, name, created_on from students order by created_on;
 ```
 **Вывести id пользователя, имя, дату создания пользователя. Отсортировать по порядку убывания даты добавления пользоватлеля.**
 ```SQL
select id, name, created_on from students order by created_on desc;
 ```
