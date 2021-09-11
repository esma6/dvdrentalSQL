# dvdrentalSQL
--film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?    
  ```
    Select AVG(retanl_rate) from film;  
  ```  
--film tablosunda bulunan filmlerden kaçtanesi 'C' karekteri ile başlar?  
```
    SELECT COUNT(*) FROM film WHERE title LIKE 'C%'; 
  ``` 
--film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?  
```
  Select MAX(length) from film where rental_rate=0.99 ;
  ```  
--film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?   
```
 Select COUNT (DISTINCT(replacement_cost)) from film where length>150 ;
 ``` 
