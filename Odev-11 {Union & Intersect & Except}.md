# Odev-11 {Union & Intersect & Except}

Type: ODEVLER

1. **actor** ve **customer** tablolarında bulunan **first_name** sütunları için tüm verileri sıralayalım.
    
    ```sql
    SELECT first_name FROM customer
    UNION
    SELECT first_name FROM actor;
    ```
    
2. **actor** ve **customer** tablolarında bulunan **first_name** sütunları için kesişen verileri sıralayalım.
    
    ```sql
    SELECT first_name FROM customer
    INTERSECT
    SELECT first_name FROM actor;
    ```
    
3. **actor** ve **customer** tablolarında bulunan **first_name** sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım.
    
    ```sql
    SELECT first_name FROM customer
    EXCEPT
    SELECT first_name FROM actor;
    ```
    
4. İlk 3 sorguyu tekrar eden veriler için de yapalım.
    
    ```sql
    SELECT first_name FROM customer
    UNION ALL
    SELECT first_name FROM actor;
    *******************
    SELECT first_name FROM customer
    INTERSECT ALL
    SELECT first_name FROM actor;
    *******************
    SELECT first_name FROM customer
    EXCEPT ALL
    SELECT first_name FROM actor;
    ```