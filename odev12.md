# dvdrentalSQL
--film tablosunda film uzunluğu length sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?    
  ```
Select COUNT(*) from film where length>(Select avg(length) from film);
  ```  
--film tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?   
```
Select COUNT(*) from film WHERE rental_rate = (SELECT MAX(rental_rate) FROM film); 

  ``` 
--film tablosunda en düşük rental_rate ve en düşün replacement_cost değerlerine sahip filmleri sıralayınız.  
```Select * from film where rental_rate=(Select min(rantal_rate) from film) AND replacement_cost=(Select min(replacement_cost) from film);
  ```  
--payment tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.   
```
SELECT customer_id,COUNT(customer_id) AS total_transactions
FROM payment
GROUP BY customer_id
ORDER BY total_transactions DESC
LIMIT 3;
 ```  
