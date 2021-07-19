## MacChanger
<strong>Projenin Özeti</strong>
<p>Debian/Ubuntu tabanlı işletim sistemleri için terminal üzerinden bu uygulama çalıştırılıp verilen iki adet input(arg) ile cihazın harici/dahili wifi kartı veya kendi ethernet adaptörü için MAC adresi değiştirilmesini sağlar.</p>

<strong>Uygulama içerisinde kullandığım kütüphaneler ve işlevlerinin özeti</strong><br>
  <p>subprocess ve optparse kütüphaneleri kullanıldı;<br>
<p>• subproccess > Uygulama içerisinde yazılacak kodu terminalde (veya Command Prompt) çalıştırarak bilgisayarımıza komut vermeye yarıyor. <br>
  Örneğin "ls" komutunu uygulama içerisinde çağırabiliyor ve çıktıları yazdırabiliyoruz.<br>
<p>• optparse > Terminal/Command Prompt üzerinde kullanıcıdan input alma işlemi için kullanıldı.<br>
  Kullanıcıdan alınan argümanların sistem üzerinde uygulanıp kaydedilebilmesi için kullanıldı.<br>
  Bu kütüphanenin kullanılabilmesi için bir obje oluşturma şartı vardır. Uygulama içerisinde bu objeyi "parse_pbject" olarak tanımladım.<br>
  Argümanların kaydedilmesi için; "dest=interface", "help=interface to change" yani dest ve help kwargs kullanıldı.</p><br>
  
<strong>Uygulama nasıl çalıştırılır ?</strong><br>
<p>Terminal/Command Prompt üzerinden uygulamanın bulunduğu dizine gidilir,</p>

#python my_mac_changer.py -i <İşlemin Yapılacağı Ethernet Arayüzü> -m <Yeni MAC Adresimiz>
## OR
##python3 my_mac_changer.py -i <İşlemin Yapılacağı Ethernet Arayüzü> -m <Yeni MAC Adresimiz>
