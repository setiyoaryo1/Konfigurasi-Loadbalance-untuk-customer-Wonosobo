# Konfigurasi-Loadbalance-untuk-customer-Wonosobo

Nama saya Setiyo Aryo Winata. Pada repositori ini, saya mendokumentasikan konfigurasi Load Balance dengan metode PCC (Per Connection Classifier) pada perangkat MikroTik.

Konfigurasi ini diterapkan untuk kebutuhan pelanggan yang menggunakan dua koneksi internet, yaitu:

ISP 1 dengan bandwidth 100 Mbps

ISP 2 dengan bandwidth 50 Mbps

Tujuan dari konfigurasi ini adalah untuk mengoptimalkan distribusi trafik internet secara seimbang dan stabil, dengan tetap menjaga kestabilan koneksi pada sesi tertentu seperti login, streaming, maupun VPN.


```shell
/ip firewall nat
add chain=srcnat out-interface=WAN1 action=masquerade`



