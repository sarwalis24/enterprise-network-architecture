# Dokumentasi Arsitektur Jaringan Enterprise (PT Jaya Maju)

## Deskripsi Proyek
Simulasi jaringan skala enterprise yang dirancang menggunakan **Cisco Packet Tracer** untuk menghubungkan kantor pusat dan cabang dengan menerapkan manajemen IP *Subnetting*, protokol *Routing* Dinamis, serta pembagian VLAN yang terstruktur guna mengamankan lalu lintas data perusahaan.

## Komponen & Topologi
- **Router Utama:** Cisco 2911 / ISR G2
- **Switch:** Cisco Catalyst 2960 (Access & Distribution Layer)
- **End Devices:** PC, Laptop, dan Server Perusahaan
- **Protokol Routing:** OSPF / Static Routing

## Rangkuman Konfigurasi Routing (Contoh)
```text
Router_Pusat> enable
Router_Pusat# configure terminal
Router_Pusat(config)# router ospf 1
Router_Pusat(config-router)# network 192.168.10.0 0.0.0.35 area 0
Router_Pusat(config-router)# network 10.0.0.0 0.0.255.255 area 0
Router_Pusat(config-router)# exit
