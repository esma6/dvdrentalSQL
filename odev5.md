# dvdrentalSQL
--film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en uzun (length) 5 filmi sıralayınız.     
  ```
    Select * from film where title like '%n' ORDER BY length DESC;  
  ```  
--film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en kısa (length) ikinci 5 filmi sıralayınız.  
```
      Select * from film where title like '%n' ORDER BY length ASC; 
  ``` 
--customer tablosunda bulunan last_name sütununa göre azalan yapılan sıralamada store_id 1 olmak koşuluyla ilk 4 veriyi sıralayınız.  
```
  Select * from customer where sotere_id=1 Order By last_name DESC LIMIT 4;
  ```  
