## Man Komutu ile Detaylı Arşivleme
Bu komutların kullanımını daha iyi anlamak için, man komutunu kullanarak her biri hakkında ayrıntılı bilgi edinebilirsiniz.
**man** (manual) komutu, Linux ve Unix tabanlı işletim sistemlerinde bulunan bir komuttur ve diğer komutların kullanımı hakkında bilgi içeren kılavuzları gösterir. **man** komutu, kullanıcılara sistemin komutlarını, dosyalarını, kütüphanelerini, işlemlerini, ayarlarını ve diğer önemli öğeleri hakkında ayrıntılı bilgi sağlar.
**man** komutunu kullanarak aşağıdaki gibi kullanabilirsiniz:
```sh 
man komut_adı
```
Arşivleme komutlarının temel parametreleri aşağıdaki gibidir.
-c: Arşiv oluşturma modu
-x: Arşivden çıkarma modu
-v: İşlem sırasında detaylı çıktılar verir
-f: Arşiv dosyasının adını belirler
-z: Gzip ile sıkıştırma yapar
-j: Bzip2 ile sıkıştırma yapar
-J: Xz ile sıkıştırma yapar

man gzip komutunu kullanarak, gzip komutunun kullanımını ve tüm seçeneklerini görebilirsiniz. Örneğin, -c seçeneği ile sıkıştırılmış dosyanın standart çıkışa yazdırılmasını sağlayabilirsiniz:
```sh 
man gzip
```