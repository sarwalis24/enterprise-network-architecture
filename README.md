# Enterprise Network Architecture (PT Jaya Maju)

Simulasi perancangan arsitektur jaringan skala perusahaan (*Enterprise*) yang dikembangkan menggunakan **Cisco Packet Tracer**. Proyek ini dirancang untuk mengoptimalkan manajemen pengalamatan IP (*Subnetting*), pengaturan protokol *Routing*, serta pembagian *VLAN* guna mengamankan lalu lintas data perusahaan.

## 📁 Daftar Isi File di Repository Ini
- **Topologi Jaringan (.pkt):** File simulasi utama Cisco Packet Tracer untuk PT Jaya Maju.
- **Gambar Topologi (.png / .jpg):** Dokumentasi visual struktur jaringan yang terhubung.
- **Dokumentasi Konfigurasi:** Catatan pengaturan IP, *Switching*, dan *Routing*.

## ⚙️ Ringkasan Konfigurasi Routing (OSPF)
```text
Router_Pusat> enable
Router_Pusat# configure terminal
Router_Pusat(config)# router ospf 1
Router_Pusat(config-router)# network 192.168.10.0 0.0.0.35 area 0
Router_Pusat(config-router)# network 10.0.0.0 0.0.255.255 area 0
Router_Pusat(config-router)# exit
Router_Pusat(config)# exit
Router_Pusat# write memory
