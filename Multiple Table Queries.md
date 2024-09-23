#Week3

Vivek Sharma

###Question 1

select country.name as "country name", airport.name as "airport name"  from country, airport 
where airport.iso_country = country.iso_country and country.name = "Iceland";
![img_10.png](img_10.png)


###Question 2

select airport.name as "Airport Name" from airport,country where airport.iso_country = country.iso_country and country.name = "France" and airport.type = "large_airport";
![img_11.png](img_11.png)


###Question 3

Select country.name as "country_name", airport.name as "airport_name" from airport,country where airport.iso_country = country.iso_country and country.continent = "AN";
![img_12.png](img_12.png)


###Question 4

select elevation_ft from airport,game where game.location = ident and screen_name ="Heini";
![img_13.png](img_13.png)


###Question 5

select elevation_ft * 0.3048 as "elevation_m" from airport,game where game.location = ident and screen_name ="Heini";
![img_14.png](img_14.png)


###Question 6

select name from airport,game where location = ident and screen_name = "Ilkka";
![img_15.png](img_15.png)


###Question 7

select country.name from airport,country,game where airport.iso_country = country.iso_country and location = ident and screen_name = "Ilkka";
![img_16.png](img_16.png)


###Question 8

select name from goal, goal_reached, game where game_id and goal.id = goal_id and screen_name = "Heini";
![img_17.png](img_17.png)


###Question 9

select airport.name from game, goal_reached, goal, airport where ident = location and game.id = game_id and goal.id = goal_id and screen_name = "Ilkka" and goal.name = "CLOUDS";
![img_18.png](img_18.png)


###Question 10

select country.name from game, goal_reached, goal, country, airport where airport.iso_country = country.iso_country and ident = location and game.id = game_id and goal.id = goal_id and screen_name = "Ilkka" and goal.name = "CLOUDS";
![img_19.png](img_19.png)