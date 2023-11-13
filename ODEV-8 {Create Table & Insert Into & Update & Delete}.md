# ODEV-8 {Create Table & Insert Into & Update & Delete}

Type: ODEVLER

1. **test** veritabanınızda **employee** isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
    
    Databases dosyasina sag tiklanarak “Create Database” denir.Sonrasinda olusan database’e sag tiklanarak Query Tool acilir.Asagidaki sorgu yazilir.
    

```sql
CREATE TABLE employee(
	id INTEGER,
	name VARCHAR(50),
	birthday DATE,
	email VARCHAR(100)
);
```

1. Oluşturduğumuz **employee** tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
    
    ![Screenshot 2023-11-14 at 00.05.31.png](ODEV-8%20%7BCreate%20Table%20&%20Insert%20Into%20&%20Update%20&%20Dele%20cef7db252b984aedb636aabd1f6d61b7/Screenshot_2023-11-14_at_00.05.31.png)
    
2. Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

```sql
UPDATE employee
SET id=1,
	name='Jasmin',
	birthday='1999-09-03',
	email='jasmin@gmail.com'
WHERE id=1;
***************************

UPDATE employee
SET email='xxxxx@gmail.com'
WHERE birthday > '1999-01-01';
```

1. Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

```sql
DELETE FROM employee
WHERE email = 'xxxxx@gmail.com';
```