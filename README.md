# -ODEV6-SQL
dvdrental sorgu senaryoları çözümleri
SORGU 1- film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?
ÇÖZÜM 1- SELECT ROUND(AVG(rental_rate), 2) FROM film;
<img width="515" alt="Ekran Resmi 2023-03-03 16 23 17" src="https://user-images.githubusercontent.com/116847744/222731164-fa8c33ba-ea8c-4477-9adc-e5c21a32ab4b.png">

SORGU 2- film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?
ÇÖZÜM 2- SELECT COUNT(title) FROM film
WHERE title LIKE 'C%';
<img width="517" alt="Ekran Resmi 2023-03-03 16 24 58" src="https://user-images.githubusercontent.com/116847744/222731524-e45a081d-3fbc-4128-9cae-8b06db2a3084.png">

SORGU 3- film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?
ÇÖZÜM 3- SELECT MAX(length) FROM film
WHERE rental_rate = 0.99;
<img width="549" alt="Ekran Resmi 2023-03-03 16 26 31" src="https://user-images.githubusercontent.com/116847744/222731812-aa6f5ba4-573e-4755-9e45-4417e183ff4d.png">

SORGU 4- film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?
ÇÖZÜM 4- SELECT COUNT(DISTINCT (replacement_cost)) FROM film
WHERE length > 150;
<img width="573" alt="Ekran Resmi 2023-03-03 16 34 08" src="https://user-images.githubusercontent.com/116847744/222733359-38385c41-f004-49ac-8e71-35f77a6b1907.png">
