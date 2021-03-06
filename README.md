# MultiBoot Utility Tr-En


![alt MultiBoot Utility](https://github.com/MultiBoot-Utility/MultiBoot-Utility/blob/master/MultiBoot%20Utility/Goruntuler/MultiBoot_Utility_1_Tr.PNG)

## Download
#### Turkish (v1.7)
[![Download MultiBoot Utility](https://a.fsdn.com/con/app/sf-download-button)](https://sourceforge.net/projects/multiboot-utility/files/MultiBoot%20Utility%20Tr.exe/download)

#### English (v1.7)
[![Download MultiBoot Utility](https://a.fsdn.com/con/app/sf-download-button)](https://sourceforge.net/projects/multiboot-utility/files/MultiBoot%20Utility%20En.exe/download)

[Eski Versiyonlar](https://github.com/MultiBoot-Utility/MultiBoot-Utility/tree/master/MultiBoot%20Utility/Old)

## Detaylı Bilgi

[www.tnctr.com](https://www.tnctr.com/topic/642741-multiboot-utility-v10/)

[sourceforge.net](https://sourceforge.net/p/multiboot-utility/)

## Kullanım Amaçları

#### USB/HDD lerde;
* Grub2 kurulumu yapar. Boot olacak şekilde hazır duruma getirir.
	- ÖNEMLİ * Boot dizinini olarak istediğiniz isimdeki bir klasörü seçebilirsiniz.
* Kullanılan mevcut MultiBoot sistemlerde Grub2 versiyon güncellemesi yapar.
	- İster program üzerinde gömülü Grub2 dosyalarla, isterseniz kendi indirmiş olduğunuz Grub2 dosyaları ile güncelleme yapabilirsiniz.
	- Güncelleme işlemini Legacy, Efi32 ve Efi64 ayrı ayrı seçmeli olarak yapabilirsiniz.
* Grub2 v2.04 ve v2.05 için g2ldr, core.img, bootia32.efi ve bootx64.efi dosyalarını oluşturarak sisteminizdeki ilgili yerlere kopyalar.
* Grub2 Dosya Yönetici kurulumu yapar. Kullanıma hazır hale getirir.
* Clover Bootloader'ın en güncel versiyonunu indirir ve kullanılan mevcut MultiBoot sistemine entegre ederek kullanmaya hazır hale getirir.
	- Güncel dosyaları internetten indirdiği için internet bağlantısı gerekmektedir.
	- Sistemde Clover Bootloader dosyaları varsa en güncel versiyon olarak günceller.
	- Sistemde Clover Bootloader yoksa en güncel versiyonu kurar ve kullanıma hazır hale getirir.
* rEFInd Bootloader'ın en güncel versiyonunu indirir ve kullanılan mevcut MultiBoot sistemine entegre ederek kullanmaya hazır hale getirir.
	- Güncel dosyaları internetten indirdiği için internet bağlantısı gerekmektedir.
	- Sistemde rEFInd Bootloader dosyaları varsa en güncel versiyon olarak günceller.
	- Sistemde rEFInd Bootloader yoksa en güncel versiyonu kurar ve kullanıma hazır hale getirir.
* Kullanılan mevcut MultiBoot sistemine güncel Grub4Dos dosyalarını indirir ve kullanmaya hazır hale getirir.
	- Güncel dosyaları internetten indirdiği için internet bağlantısı gerekmektedir.
	- Sistemde Grub4Dos hiç yoksa default olarak grub dizininin altına kurar.
	- Sistemde önceden yüklü Grub4Dos dosyaları varsa (Hangi klasörde olduğu önemli değil) üzerine yazarak güncelleme yapar.
* UEFI de Secure Boot aktif iken boot sorunu yaşanması durumunda kullanılan mevcut MultiBoot sisteminin UEFI boot yöntemini Microsoft tarafından imzalanmış orijinal efi dosyaları ile değiştirir ve kullanıma hazır hale getirir.
* XorBoot Bootloader kurulumu yapar. Kullanıma hazır hale getirir.
	- Xorboot Bootlader yapılandırma programlarını direk program üzerinden kullanabilirsiniz.
* Program üzerinden direk Sanal Disk Yönetim programı, QEMU Test programı ve Bootice programını açarak bütün testleri yapabilirsiniz.

## Yapılan Değişiklikler
```
(v1.7)
 # Hata düzeltmesi (grubenv)
 
(v1.6)
 # Grub2 Dosya Yönetici için en son güncel dosyaların internetten indirilerek kurulumu sağlandı.
 # Sıfır kurulumda Grub2 Dosya Yönetici ve Grub4Dos dosyalarının en güncel dosyalarının kullanılması sağlandı.

(v1.5)
 # Sıfır kurulum v2.04 ve v2.05 seçmeli hale getirildi.
 # Xorboot bootloader eklendi.
 # Program üzerinden XorBoot Bootloader programlarının kullanılması sağlandı.
 # Loader oluşturmada ve güncelleştirmede grubx64.efi ve grubia32.efi dosyalarınında oluşturulması sağlandı.
 # Windows kullanıcı adında boşluk olduğunda kurulumda oluşan hata giderildi.
 
(v1.4)
 # Clover ve rEFInd Bootloader eklendi.
 # Disk yapısı bilgisi eklendi.
 
(v1.3)
 # Windows kurulu sürücüde işlem yapılması seçimli hale getirildi.
 
(v1.2)
 # Program ilk açılış sonrasındaki açılışlarda versiyon değişikliği olmadığı müddetçe direk açılması sağlandı.

(v1.1)
 # Seçilen sürücüde Windows yüklü ise işlemlerin yapılması engellendi.
 # Grub4Dos için işlem tamamlandıktan sonra gelen hata giderildi.

(v1.0)
 # Programın ilk sürümü yayınlandı.
 ```