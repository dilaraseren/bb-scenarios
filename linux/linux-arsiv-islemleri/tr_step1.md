## Linux Arşiv İşlemleri
Linux'da dosya ve dizinleri sıkıştırmak için birçok komut mevcuttur. Bu komutlar sayesinde dosya boyutlarını küçültebilir, disk alanı tasarrufu sağlayabilir ve dosya aktarımı sırasında bant genişliği kullanımını azaltabilirsiniz. 

1- gzip: gzip, en yaygın kullanılan sıkıştırma programlarından biridir. gzip, dosyaları tek tek sıkıştırır ve .gz uzantısıyla kaydeder. Aşağıdaki komutla **dosya.txt** dosyası oluşturup  dosyayı gzip ile sıkıştırabilirsiniz:
```sh 
touch dosya.txt
gzip dosya.txt
```

2- bzip2: bzip2, dosyaları gzip'a göre daha iyi sıkıştırır ve daha küçük dosya boyutları sağlar. bzip2 çoğu linux dağıtımında default geliyor. Ancak kurulu değilse aşağıdaki komut ile kurabilirsiniz:
```sh 
yum install bzip2 
```
Aşağıdaki komutla **dosya.txt** dosyası oluşturup  dosyayı bzip2 ile sıkıştırabilirsiniz:
```sh 
touch dosya.txt
bzip2 dosya.txt
```
3- xz: xz, dosyaları oldukça yüksek bir oranda sıkıştırır ve en düşük dosya boyutlarını sağlar. xz sıkıştırma işlemi yapmak için **xz-utils** adlı paketin kurulu olması gerekir. Eğer xz-utils paketi kurulu değilse, aşağıdaki komutları kullanarak kurabilirsiniz:
```sh 
yum install xz-utils
```
Aşağıdaki komutla **dosya.txt** dosyası oluşturup  dosyayı xz ile sıkıştırabilirsiniz:
```sh 
touch dosya.txt
xz dosya.txt
```
4- tar: tar, birden fazla dosyayı bir araya getirerek sıkıştırmak için kullanılır. Aşağıdaki komutla dosyaları tar ile sıkıştırabilirsiniz:
```sh 
touch dosya1.txt dosya2.txt dosya3.txt
tar -czvf dosyalar.tar.gz dosya1.txt dosya2.txt dosya3.txt
```
Bu komut, dosya1.txt, dosya2.txt ve dosya3.txt dosyalarını tek bir dosya olan dosyalar.tar.gz' ye sıkıştırır.
**-x** seçeneği, bir arşiv dosyasını açmak ve dosyaları çıkarmak için kullanılır:
```sh 
tar -xzvf  dosyalar.tar.gz
```
Bu komutların her biri farklı sıkıştırma oranlarına ve performanslara sahiptir. Dosya boyutunu azaltmak veya dosya aktarımı sırasında bant genişliği kullanımını azaltmak için en uygun komutu seçebilirsiniz.



