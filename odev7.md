# dvdrentalSQL
--film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.   
  ```
    Select rating
    From film
    Group By rating;
  ```  
--film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.  
```
    Select replacement_cost,COUNT(*)
    FROM film
    Group By replacement_cost
    HAVING COUNT(*)>50;
  ``` 
--customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?  
```
  SELECT store_id,COUNT(*)
  From customer
  Group By store_id;
  ```  
--city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıra country_id bilgisini ve şehir sayısını paylaşınız.  
```
 Select country_id,COUNT(*)
 From city
 Group By country_id
 ORDER BY COUNT(*) DESC
 LIMIT 1;
 ``` 
