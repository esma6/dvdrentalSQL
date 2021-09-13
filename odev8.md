# dvdrentalSQL
--test veritabanınızda employee isimli sütun bilgileri id (INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.  
  ```
   CREATE TABLE employee (
	id INTEGER,
	name VARCHAR(50), 
	birthday DATE, 
	email VARCHAR(100) );
  ```  
--2.Oluşturduğumuz employee tablosuna Mockaroo servisini kullanarak 50 adet veri ekleyelim.    
```
  ``` 
--Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.  
```
UPDATE employee
SET 
	name = 'lorem ipsum', 
	birthday = '1980-01-01', 
	email = 'lorem@ipsum.com' 
WHERE id = 1;
-----------------
UPDATE employee  
SET
	name = 'lorem ipsum',
	birthday = '1980-01-01',
	email = 'lorem@ipsum.com'
WHERE name LIKE 'A%';
-----------------
UPDATE employee  
SET
	name = 'lorem ipsum',
	birthday = '1980-01-01',
	email = 'lorem@ipsum.com'
WHERE birthday BETWEEN '1990-01-01' AND '1995-01-01'; 
  ```  
--Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.   
```
DELETE FROM employee 
WHERE birthday BETWEEN '1970-01-01' AND '1995-01-01';
-----------------
DELETE FROM employee 
WHERE name LIKE 'A%';
-----------------
DELETE FROM employee 
WHERE name LIKE 'Sa%' AND
birthday < '2000-01-01';
-----------------
DELETE FROM employee 
WHERE email LIKE 'a%' AND
birthday BETWEEN '1981-01-01' AND '2004-01-02';
 ``` 
