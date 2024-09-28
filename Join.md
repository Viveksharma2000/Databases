#Week4

Vivek Sharma

###Question 1

Select country.name as "country name", airport.name As "airport name" from country join airport ON country.iso_country=airport.iso_country where country.name="finland";
![img_20.png](img_20.png)


###Question 2

select game.screen_name as "screen_name",airport.name as "name" from game join airport on game.location = airport.ident;
![img_21.png](img_21.png)


###Question 3

SELECT game.screen_name AS "screen_name",  country.name AS "name" FROM game JOIN airport ON game.location = airport.ident JOIN country ON airport.iso_country = country.iso_country;
![img_22.png](img_22.png)


###Question 4

SELECT airport.name AS "Airport Name", game.screen_name as "Player Name" FROM airport LEFT JOIN game on game.location = airport.ident WHERE airport.name LIKE '%Hels%';
![img_23.png](img_23.png)


###Question 5

SELECT goal.name, game.screen_name FROM goal LEFT JOIN goal_reached ON goal.id = goal_reached.goal_id LEFT JOIN game ON goal_reached.game_id = game.id;
![img_24.png](img_24.png)