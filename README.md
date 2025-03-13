# MarLing

Ini adalah [Marzban](https://github.com/Gozargah/Marzban) yang sudah saya tambahkan nginx untuk konfigurasi koneksi WebSocket dan XHTTP pada single port. </br>
WebSocket sudah support untuk 443 TLS, 80 HTTP dan Wildcard path, contoh /enter-your-custom-path/trojan </br>
XHTTP sudah support untuk 443 TLS Quic </br>

Disclaimer: Proyek ini hanya untuk pembelajaran dan komunikasi pribadi, mohon jangan menggunakannya untuk tujuan ilegal. </br>
Credit aplikasi full to [Gozargah Marzban](https://github.com/Gozargah), saya hanya edit sedikit untuk instalasi sederhana bagi pemula . </br>

# Special Thanks to
- [Gozargah](https://github.com/Gozargah/Marzban)
- [hamid-gh98](https://github.com/hamid-gh98)
- [x0sina](https://github.com/x0sina/marzban-sub)

# List Protocol yang support
- VLess
- VMess
- Trojan

# Yang harus dipersiapkan
- VPS dengan minimal spek 1 Core 1 GB ram
- Domain yang sudah di pointing ke CloudFlare
- Pemahaman dasar perintah Linux

# Sistem VM yang dapat digunakan
- Debian 11 </br>
- Debian 12 [**RECOMMENDED**] </br>
- Ubuntu 20.04 </br>

# Instalasi
  ```html
 apt-get update && apt-get upgrade -y && apt dist-upgrade -y && update-grub
 ```
Pastikan anda sudah login sebagai root sebelum menjalankan perintah dibawah
 ```html
 apt install curl jq wget -y && wget https://raw.githubusercontent.com/xsm-syn/marzban/main/install.sh && chmod +x install.sh && screen -S setup ./install.sh
 ```

Buka panel Marzban dengan mengunjungi https://domainmu/dashboard <br>

Jika ingin mengubah konfigurasi env variable 
```html
marzban edit-env
 ```
Perintah Restart service Marzban 
```html
marzban restart
 ```
Perintah Cek Logs service Marzban 
```html
marzban logs
 ```
Perintah ganti Core Xray marzban
```html
marzban core-update
 ```
Perintah untuk sett backup marzban
```html
 marzban backup-service
 ```
Perintah Cek update service Marzban
```html
marzban update
 ```
Perintah untuk ke Menu Warp
```html
warp
 ```
atau selebih nya bisa cek 
```html
warp --help
 ```

Jika ada typo atau saran bisa PM ke saya di :<a href="https://t.me/after_sweet" target=”_blank”><img src="https://img.shields.io/static/v1?style=for-the-badge&logo=Telegram&label=Telegram&message=Click%20Here&color=blue"></a><br>
