
```
Önemli Not!
Türkiye'nin 81 ili ve ilçeleri örnek olarak mevcuttur ancak 
kullanımdan doğabilecek sorunlar kullanan kişiye aittir, 
lütfen gerekli kontrollerinizi yapınız!
```

#### Ne Yapıyor?

Önce Şehir seçmenizi istiyor, seçilen şehrin ilçelerini getiriyor

#### Basitçe Nasıl Yapıyor?
````
1) tr-il-ilce.json veri tabanında il ve ilçeler bulunuyor
2) "Fetch" ile veri tabanındaki sehirler alınıyor ve app dataya yazılıyor
3) v-for ile şehirler ve indexleri selectbox ta listeleniyor
4) ilçeler select boxı bu sırada nul döndüğü için v-if ile ekrana basılmıyor
5) Seçim yapıldığında v-model ile seçilen kayıtın indexi secilenil ile atanıyor ve anı zamanda ilcegetir fonksiyonu çalıştırılıyor
6) ilçe getir fonksiyonu v-model üzerinden indeksi alıyor seçilen sehrin ilçelerini app datadaki ilceler'e atıyor ilçeler select box artık  null olmadığı için v-if koşulu ortadan kalkıyor, böylece ilçeler selectbox'ı ekrana basılıyor
````  