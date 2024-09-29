#Week5

Vivek Sharma

###Question 1

select max(elevation_ft) from airport;
![img_30.png](img_30.png)


###Question 2

select continent, count(*) from country group by continent;
![img_31.png](img_31.png)


###Question 3

select screen_name, count(*) from game, goal_reached where id = game_id group by screen_name;
![img_32.png](img_32.png)


###Question 4

select screen_name from game where co2_consumed in(select min(co2_consumed) from game );
![img_33.png](img_33.png)


###Question 5

select country.name, count(*) from airport, country where airport.iso_country = country.iso_country group by country.iso_country order by count(*) desc limit 50;
![img_34.png](img_34.png)


###Question 6
select country.name from airport, country where airport.iso_country = country.iso_country group by country.iso_country having count(*) > 1000;
![img_35.png](img_35.png)


###Question 7

select name from airport where elevation_ft in ( select max(elevation_ft) from airport );
![img_36.png](img_36.png)


###Question 8

select name from country where iso_country in ( select iso_country from airport where elevation_ft in( select max(elevation_ft) from airport ) );
![img_37.png](img_37.png)


###Question 9

select count(*) from game, goal_reached where id = game_id and screen_name = "Vesa" group by screen_name;
![img_38.png](img_38.png)


###Question 10

select name from airport where latitude_deg in( select min(latitude_deg) from airport );
![img_39.png](img_39.png)