# **Praktikum Jaringan komputer**

# *Tugas Akhir 2 Build a Switch and Router Network*

## Video Demonstrasi  
[🔗 Klik di sini untuk menonton video praktikum di YouTube](https://youtu.be/a2p46yNuHQk)


## File Cisco Packet Tracer  
**TA 2** `TA2.pkt`  
[Klik di sini untuk mengunduh file Cisco Packet Tracer](Judul\ 2/TA2.pkt)

## Topologi Jaringan  
Berikut adalah tampilan topologi jaringan yang digunakan pada praktikum ini:
(<img width="570" height="147" alt="image" src="https://github.com/user-attachments/assets/d846952a-83c0-4309-ae5d-e81e9ee5c858" />)

## Deskripsi Singkat  
Pada praktikum ini dilakukan konfigurasi dasar antara **switch** dan **router** menggunakan Cisco Packet Tracer. Tujuannya adalah agar setiap perangkat dalam jaringan dapat saling berkomunikasi melalui konfigurasi IP dan routing sederhana.

## Hasil Uji 
# Ping PC-B From PC-A
Pada awal pengujian, komunikasi antar subnet belum berhasil dilakukan karena antarmuka router (default gateway) belum dikonfigurasi, sehingga lalu lintas Layer 3 belum dapat dirutekan antar subnet. Setelah konfigurasi antarmuka router dilakukan, pengujian *ping* menunjukkan hasil berhasil, menandakan proses routing antar jaringan sudah berjalan dengan baik. 
<img width="869" height="889" alt="image" src="https://github.com/user-attachments/assets/7fbfc407-0133-4475-bc4a-09ffd6255a6e" />

# Ping PC-B From S1
Pengujian ini dilakukan untuk memastikan bahwa switch mampu terhubung dengan perangkat pada jaringan lain. Hasilnya menunjukkan bahwa proses *ping* berhasil, yang berarti switch dapat meneruskan permintaan ICMP melalui gateway (router) menuju jaringan tujuan. Hal ini menunjukkan bahwa router telah berhasil melakukan *routing* lalu lintas *ping* antar subnet, dan secara bawaan, switch Cisco 2960 akan otomatis mengaktifkan antarmuka yang terhubung ke perangkat. 
<img width="601" height="215" alt="image" src="https://github.com/user-attachments/assets/ec23fc50-d978-468f-acd2-6e41ebc402fe" />

## Kesimpulan  
Hasil praktikum menunjukkan bahwa konfigurasi berhasil ketika seluruh perangkat dapat melakukan *ping* antar subnet tanpa error.
