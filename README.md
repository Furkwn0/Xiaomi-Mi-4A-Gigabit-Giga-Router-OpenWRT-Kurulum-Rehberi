# Xiaomi Mi 4A Gigabit/Giga Router OpenWRT Kurulum Rehberi
Bu yöntem ile Windows üzerinde Xiaomi Mi Router 4A Gigabit/Giga routerınıza kısa sürede OpenWRT kurabileceksiniz.   
diğer marka ve model routerlarda bu yöntemi denemek cihazı (Brick) eder.
OpenWRT kurulumu cihazınızı garanti dışı bırakacak olup, oluşabilecek tüm sorunlar sizin sorumluluğunuz altında olduğunu belirtmek isteriz. 
Konu ile ilgili hiçbir sorumluluk kabul etmemekteyiz.

##  Dikkat Etmeniz Gerekenler:
- modemin stok sürümü 3.0.x ise bunu 2.28.x olan herhangi bir sürüme düşürmeniz gereklidir.
- Bu yöntem routerın V1 sürümü içindir.
- indirdiğiniz openwrt frimware.bin dosyasının ismini değiştirdikten sonra değiştirdiğiniz isme göre komut yazmanız gerekmektedir. 
- wget komudundaki ip adresini kendindi ip adresinizi yazınız Terminali a.ıp ipconfig yazdıktan sonra ipv4 kısmında yazmaktadır.

# Başlangıç
## 1) Routerimizin arkasındaki reset tuşuna basılı tutalım ve routerimizi resetleyelim ardından 192.168.31.1 veya miwifi.com adresine giderek modemimize kurulum yapalım
## 2) OpenWRT kurulumu için gerekli dosyalarımızı indirelim
- python indirelim
- https://firmware-selector.openwrt.org
- https://github.com/acecilia/OpenWRTInvasion

## 3) Gerekli dosyaları indirdikten sonra OpenWRTİnvasion dosyasını ayıklayalım 
## 4) OpenWRTİnvasion dosyasını açalım ve boş bir kısıma shifte basarak sağ tıklayalım ardından powershell penceresini açalım
### Not:Burada modemimiz internete bağlı olsun ve aşşağıdakli komutları yapıştralım
```shell
pip install -r requirements.txt
python remote_command_execution_vulnerability.py
```
<img width="810" height="452" alt="Ekran görüntüsü 2026-05-23 215138" src="https://github.com/user-attachments/assets/d519d51f-0012-447f-b2a3-4035dbc5d464" />





```
telnet <router_ip_address>
```

* User: `root`
* Password: `root`
