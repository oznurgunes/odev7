1)film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.<br><code>
  select rating, count(*) from film
group by rating;</code><br>
2)film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız."<br><code>
 select replacement_cost, count(*) from film
group by replacement_cost
having count(*) > 50;</code><br>
3) customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?<br><code>
  select store_id, count(*) from customer
group by store_id;</code><br>
4)city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıra country_id bilgisini ve şehir sayısını paylaşınız.<br><code>
  select country_id, count(*) from city
group by country_id
order by country_id desc
limit 1;
