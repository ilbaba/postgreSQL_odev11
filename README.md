# postgreSQL_odev11
PostgreSQL -  On birinci ödev - Ilgar Babashli

# _Q1_ 

actor ve customer tablolarında bulunan first_name sütunları için tüm verileri sıralayalım.

# _Ans_
(SELECT first_name FROM actor)
UNION ALL
(SELECT first_name FROM customer);

# _Q2_ 
actor ve customer tablolarında bulunan first_name sütunları için kesişen verileri sıralayalım.

# _Ans_
(SELECT first_name FROM actor)
INTERSECT
(SELECT first_name FROM customer);

# _Q3_ 
actor ve customer tablolarında bulunan first_name sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım.

# _Ans_
(SELECT first_name FROM actor)
EXCEPT
(SELECT first_name FROM customer);

# _Q4_ 
İlk 3 sorguyu tekrar eden veriler için de yapalım.

# _Ans_
