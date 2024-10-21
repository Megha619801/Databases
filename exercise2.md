#Q.no.1
select country.name as "country name", airport.name as "airport name"
from airport, country 
where country.iso_country = airport.iso_country and 
country.name = "Iceland";
![Screenshot (21)](https://github.com/user-attachments/assets/d7390f1c-c71b-4da9-b537-5630e9eb70c4)

#Q.no.2
 select airport.name as "airport name"
    -> from airport
    -> where airport.type = "large_airport" and
    -> airport.iso_country = "FR";
    ![Screenshot (22)](https://github.com/user-attachments/assets/5feb5282-37e3-4043-bec6-e2d42a0647cd)

#Q.no.3
select country.name as "country_name", airport.name as "airport_name"
from country, airport
where country.continent = airport.continent and 
country.continent = "AN" and 
country.name = "Antarctica";
![Screenshot (24)](https://github.com/user-attachments/assets/4a807369-1b95-4f94-a29c-784b5e28ec17)

#Q.no.4
select elevation_ft 
from game, airport 
where airport.ident = game.location and 
screen_name = "Heini";
![Screenshot (25)](https://github.com/user-attachments/assets/41be119c-ca4c-4054-8d50-6c9fbb7fef84)

#Q.no.5
select elevation_ft*0.3048 as "elevation_m"
    -> from game, airport
    -> where airport.ident = game.location and
    -> game.screen_name = "Heini";
    ![Screenshot (26)](https://github.com/user-attachments/assets/e5844d62-4458-4b66-bbf6-d0e65cdbeaa9)

#Q.no.6
select airport.name 
from airport, game 
where airport.ident = game.location and 
screen_name = "Ilkka";
![Screenshot (28)](https://github.com/user-attachments/assets/2b4a70ec-490b-40be-bdbc-603d851ff84a)

#Q.no.7
select country.name
    -> from country, game, airport
    -> where airport.ident = game.location and
    -> country.iso_country = airport.iso_country and
    -> game.screen_name = "Ilkka";
![Screenshot (29)](https://github.com/user-attachments/assets/e7200643-0565-4471-965e-f55b6fe2c4d2)

#Q.no.8
 select goal.name
    -> from goal, game, goal_reached
    -> where goal.id = goal_id and
    -> game.id = game_id and
    -> screen_name = "Heini";
![Screenshot (30)](https://github.com/user-attachments/assets/965437cd-c317-4582-b199-10e7174ed0e5)

#Q.no.9
select airport.name 
from airport, game, goal, goal_reached
where airport.ident = game.location and 
game.id = game_id and 
goal.id = goal_id and
screen_name = "Ilkka";
![Screenshot (31)](https://github.com/user-attachments/assets/4efcc3e3-2ae7-437e-b8c6-af2d7b6f0e69)

#Q.no.10
select country.name 
from country, game, goal, goal_reached, airport
where airport.ident = game.location and
country.iso_country = airport.iso_country and 
game.id = game_id and
goal.id = goal_id and
screen_name = "Ilkka";
![Screenshot (33)](https://github.com/user-attachments/assets/142d19eb-2299-4627-b7d2-96f85514fb35)









