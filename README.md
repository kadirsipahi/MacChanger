## MacChanger
<strong>Projenin Özeti</strong>
<p>Debian/Ubuntu tabanlı işletim sistemleri için terminal üzerinden bu uygulama çalıştırılıp verilen iki adet input(arg) ile cihazın harici/dahili wifi kartı veya kendi ethernet adaptörü için MAC adresi değiştirilmesini sağlar.</p>

<strong>Uygulama içerisinde kullandığım kütüphaneler ve işlevlerinin özeti</strong><br>
  subprocess ve optparse kütüphaneleri kullanıldı;
• subproccess > Uygulama içerisinde yazılacak kodu terminalde (veya Command Prompt) çalıştırarak bilgisayarımıza komut vermeye yarıyor. 
  Örneğin "ls" komutunu uygulama içerisinde çağırabiliyor ve çıktıları yazdırabiliyoruz.
• optparse > Terminal/Command Prompt üzerinde kullanıcıdan input alma işlemi için kullanıldı.
  Kullanıcıdan alınan argümanların sistem üzerinde uygulanıp kaydedilebilmesi için kullanıldı.
  Bu kütüphanenin kullanılabilmesi için bir obje oluşturma şartı vardır. Uygulama içerisinde bu objeyi "parse_pbject" olarak tanımladım.
  Argümanların kaydedilmesi için; "dest=interface", "help=interface to change" yani dest ve help kwargs kullanıldı.
  
<strong>Uygulama nasıl çalıştırılır ?</strong><br>
Terminal/Command Prompt üzerinden uygulamanın bulunduğu dizine gidilir,

#python my_mac_changer.py -i <İşlemin Yapılacağı Ethernet Arayüzü> -m <Yeni MAC Adresimiz>
## OR
##python3 my_mac_changer.py -i <İşlemin Yapılacağı Ethernet Arayüzü> -m <Yeni MAC Adresimiz>
