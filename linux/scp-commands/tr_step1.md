## Problem - SCP komutu 
Bu senaryo içerisinde sizlere tahsis edilen makinelerde belirtilen dosya dizinine ulaşmanızı ve klasörlerin içerisine aşağıdaki talimatlar gereğince SCP komutu ile dosya transferi işlemlerini uyguladığınız bir senaryo hazırlamanız istenmektedir.
### Bilgi 
SCP KOMUTU : 

SCP, "Secure Copy Protocol" (Güvenli Kopyalama Protokolü) kısaltmasıdır ve dosya transferi için kullanılan bir ağ protokolüdür. SCP, bilgisayarlar arasında güvenli bir şekilde dosya kopyalamak veya taşımak için kullanılır. Bu protokol, verilerin şifrelenmesini ve güvenli bir şekilde transferini sağlar.

SCP, çoğunlukla UNIX ve Linux işletim sistemlerinde kullanılan bir komut satırı aracıdır. 

Bu senaryoda, farklı node'lar arasında dosya transferi yapacağız.

### Talimatlar
1. node1 ve node2 sunucularında `/home` dizinine gidin.
2. node1 sunucusunda `exp.txt`, node2 sunucusunda `expm.txt` dosyalarını oluşturun.  
3. node2 sunucusundaki expm.txt dosyasını `SCP` komut yoluyla node1 sunucusuna gönderin. 
4. SCP komutu sayesinde sunucular arası dosya transferinde bulunurken karşınıza çıkan güvenlik ile ilgili soruyu YES olarak cevaplandırdıktan sonra dosya transferinin başarılı bir şekilde gerçekleştiğini ve ardından node1 sunucusuna gelerek `expm.txt` dosyasının var olduğunu kontrol edebilirsiniz.
5. İşlemleri tamamladıktan sonra "Kontrol Et" butonuna basınız ve senaryoyu tamamlayınız.

### Başarılı Çıktı
 Koşul:  
``` echo
[root@node1 ~]$ cat backup.sql
```  


