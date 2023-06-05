## Problem - Backup Alma 
Bu senaryo içerisinde sizlere tahsis edilen makinelerde belirtilen dosya dizinine ulaşmanızı ve klasörlerin içerisine aşağıdaki talimatlar gereğince backup işlemlerini uyguladığınız bir senaryo hazırlamanız istenmektedir.
### Bilgi 
Backup işlemi, bir veritabanının veya verilerin yedeklenmesi anlamına gelir. Bir yedekleme, verilerinizi korumak ve olası veri kaybı durumunda verileri geri yüklemek için önemli bir adımdır.
PostgreSQL'de backup işlemi, veritabanının mevcut durumunu kopyalayarak bir yedekleme dosyası oluşturmayı içerir. Bu yedekleme dosyası, veritabanının verilerini, tablolarını, indekslerini ve diğer bileşenlerini içerir. Yedekleme dosyası, bir veritabanını başka bir sunucuya taşımak, verileri kurtarmak veya veri kaybı durumunda geri yüklemek gibi durumlarda kullanılabilir.

Bu senaryoda, Alpine imajında çalışan bir PostgreSQL veritabanı oluşturacak ve ardından bir tablo oluşturup terminal üzerinden bir yedek alacağız.

### Talimatlar
1. Ana dizinde `/home` bir dizinine gidin.
2. Postgresql veritabanını docker imajı ile ayağa kaldırabilmek için `docker run --name mypostgresdb -e POSTGRES_PASSWORD=mysecretpassword -p 5432:5432 -d postgres` komutunu çalıştıralım. 
3. Docker imajının çalıştığından emin olduktan sonra `docker exec -it mypostgresdb bash` komutunu çalıştırıp postgresql veritabanına erişelim. 
4. `psql -U postgres` komutunu çalıştırarak bağlantı gerçekleşir ve burada psql komutlarını çalıştırabilirsiniz. 
5. Postgresql veritabanına bağlandıktan sonra aşağıdaki komutları çalıştırarak tablo oluşturup terminal üzerinden bir yedek alacağız.
6. `mydatabase` adında yeni bir veritabanı oluşturun sonrasında `\c mydatabase` diyerek veritabanınıza bağlanın. 
7. Bağlantı yapıldıktan sonra yeni bir tablo oluşturunuz ve bu tabloyu da oluşturulan SQL dosyasını kullanarak tabloyu oluşturmak için `psql -U postgres -f create_table.sql` komutunu çalıştırınız ve psql içinden `\q` komutu ile çıkınız. 
8. Tablo başarıyla oluşturulduktan sonra, `pg_dump` komutunu da kullanarak bir yedek alma işlemi gerçekleştirebilirsiniz. 
9. İşlemleri tamamladıktan sonra "Kontrol Et" butonuna basınız ve senaryoyu tamamlayınız.

### Başarılı Çıktı
 Koşul:  
``` echo
[root@node1 ~]$ cat backup.sql
```  


