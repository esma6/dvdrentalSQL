# dvdrentalSQL
--film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.      
  ```
    Select DISTINCT replacement_cost from film; 
  ```  
--film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?    
```
     Select COUNT (DISTINCT (replacement_cost)) from film; 
  ``` 
--film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?   
```
  Select COUNT(*) from film WHERE title ILIKE 'T%' and rating='G';
  ```  
--country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?  
```
 Select COUNT(*)  from country where country like '_____' ;
 ```  
 --city tablosundaki şehir isimlerinin kaçtanesi 'R' veya r karakteri ile biter?  
```
 Select * from city where city like '%r';
 ```  
