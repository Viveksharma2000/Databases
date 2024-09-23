#Week3

Vivek Sharma

###Question 1

select * from goal;
![img.png](img.png)

###Question 2

select name, type from airport where iso_country="FI";
![img_1.png](img_1.png)

###Question 3

select name from airport where iso_country="FI" order by name asc;
![img_2.png](img_2.png)

###Question 4

select name, type from airport where iso_country="FI" order by type asc,name asc;
![img_3.png](img_3.png)

###Question 5

select name from country where name like "F%";
![img_4.png](img_4.png)

###Question 6

select name from country where name like "%F%";
![img_5.png](img_5.png)

###Question 7

select location from game where screen_name="Vesa";
![img_6.png](img_6.png)

###Question 8

select co2_consumed from game where screen_name="Ilkka";
![img_7.png](img_7.png)

###Question 9

select DISTINCT co2_budget from game;
![img_8.png](img_8.png)

###Question 10

select screen_name, co2_budget, co2_consumed, co2_budget - co2_consumed as co2_left from game where screen_name="Ilkka";
![img_9.png](img_9.png)