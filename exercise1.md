#question no.1
select * from goal;
![Screenshot (4)](https://github.com/user-attachments/assets/99f24dfa-b075-4238-b083-cc6e9e6e7a6f)


#question no. 2
select name, type from airport where iso_country = "FI";
![Screenshot (5)](https://github.com/user-attachments/assets/0a5ac01d-07ee-4014-9c3b-b1d2b6507daf)



#question no.3
select name, type from airport where iso_country = "FI" order by name;
![Screenshot (10)](https://github.com/user-attachments/assets/2d27da6b-5726-4e40-822d-be294e66acf7)


#question no.4
select name, type from airport where iso_country = "FI" order by type, name;
![Screenshot (11)](https://github.com/user-attachments/assets/04c3d436-8d99-430c-b36b-1db45b99b6b9)



#question no.5
select name from country where name like "F%";
![Screenshot 2024-09-12 215455](https://github.com/user-attachments/assets/3fd9a1b7-1d95-4632-819f-d968876404d2)




#question no.6
select name from country where name like "%F%";
![Screenshot 2024-09-12 215759](https://github.com/user-attachments/assets/174aac55-2721-4e96-9005-8eb2d1c7d956)





#question no.7
select location from game where screen_name = "vesa";
![Screenshot 2024-09-12 220450](https://github.com/user-attachments/assets/6a77287f-5a8d-4e2c-8e6e-b98ec13f19a8)




#question no.8
select co2_consumed from game where screen_name = "Ilkka";
![Screenshot 2024-09-12 221006](https://github.com/user-attachments/assets/a4e73460-cbdd-4569-8ba5-92682a33409a)


#question no.9
select distinct co2_budget from game;
![Screenshot 2024-09-12 221411](https://github.com/user-attachments/assets/1d156d7a-3449-4111-858d-0a6a777c1ab1)





#question no.10
select screen_name, co2_budget, co2_consumed, @co2_left:= co2_budget - co2_consumed as co2_left from game where screen_name = "Ilkka";
![Screenshot 2024-09-12 222343](https://github.com/user-attachments/assets/f517cc59-9236-457e-a876-94ab4ac616a5)









