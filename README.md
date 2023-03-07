Data - https://drive.google.com/file/d/1xdIivov7687aCJ_Hyf9QsJz2gcBnrt5r/view?usp=sharing

 Veri Seti

Tüm veri setine oran ile %80 oranında eğitim verisi 11291 fotoğraftan, %20 oranında doğrulama veri seti 2823 fotoğraftan oluşmaktadır. Veri setinde 1280 x 720 ve 640 x 640 boyutlarında 14114 fotoğraf bulunmaktadır.  Eğitim veri setinde 11907 etiketleme, doğrulama veri setinde 2910 etiketleme işlemi yapılmıştır.
Veri seti yeterli olduğu için eğitim veri setinde veri seti arttırımı uygulanmamıştır. Aynı görüntü üzerinde karşılaştırma yapmak amacıyla doğrulama veri setinde +15, -15 derece döndürme; +50, -50 parlaklık arttırma ve azaltma; +35 bulanıklık ve görüntü kırpma işlemleri uygulanmıştır. Ayrıca doğrulama veri setine helikopter ve kuş görüntüleri de eklenerek FP değeri gerçekçi şekilde denenmiştir. 

![image](https://user-images.githubusercontent.com/114474881/223410257-4f34f473-07f2-4e7c-bb9d-915af25710a6.png)

Şekil 1.1 Eğitim verisinde 11907 etiketlemenin boyutlarına göre dağılım grafiği

![image](https://user-images.githubusercontent.com/114474881/223410331-26a1be37-753e-4708-86df-8f522e6f16b5.png)

Şekil 1.2 Doğrulama verisinde 2910 etiketlemenin boyutlarına göre dağılım grafiği

YOLOv4, YOLOv4-Tiny derin öğrenme modellerinde 20000 tur(epoch) sayısında eğitilmiştir.
Eğitim sırasında eğitimi yavaşlatmamak amacıyla doğrulama veri sayısı küçük kullanılmıştır. Eğitim sonucunda elde edilen ağırlık oluşturulan %20 oranlı doğrulama veri seti ile doğruluğu ölçülmüştür.
Elde edilen grafiklerde Google Colab’ da yaşanan GPU kullanım kısıtlamasından dolayı kesintiler oluşmuştur, bu durum ağırlık verisi için bir sorun olmayıp kalınan yerden devam edilmiştir.

![hhhhhhhhhhhhhhhhhhhhhh](https://user-images.githubusercontent.com/114474881/223410836-b635ff6c-6495-456f-9b5b-c4cf32fdb0f4.jpg)

Şekil 2 YOLOv4(c), YOLOv4-Tiny(d) modellerinin iterasyona bağlı mAP ve average loss değerleri

![image](https://user-images.githubusercontent.com/114474881/223411004-8cd12698-b4e5-4e46-bbe9-c00bf7a49d66.png)

Kullanılan Sistem: 
Casper S500
İşlemci:Intel(R) Core(TM) i5-10210U CPU @ 1.60GHz, 2112 Mhz, 4 Çekirdek, 8 Mantıksal İşlemci
Ekran Kartı: NVDIA GeForce MX230
RAM: 8 GB
