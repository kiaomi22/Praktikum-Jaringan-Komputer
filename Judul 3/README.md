# **Praktikum Jaringan komputer**

# *Tugas Akhir 3 Configure VLANs and Trunking*

## Video Demonstrasi  
[🔗 Klik di sini untuk menonton video praktikum di YouTube](https://youtu.be/39BDp6FA05I)


## File Cisco Packet Tracer  
**TA 3** `TA2.pkt`  
[Klik di sini untuk mengunduh file Cisco Packet Tracer](TA3.pkt)

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
Pengujian ini dilakukan untuk memastikan bahwa switch mampu terhubung dengan perangkat pada jaringan lain. Hasilnya menunjukkan bahwa proses *ping* berhasil, yang berarti switch dapat meneruskan permintaan ICMP melalui gateway (router) menuju jaringan tujuan. Hal ini menunjukkan bahwa router telah berhasil melakukan *routing* lalu lintas *ping* antar subnet. 
<img width="601" height="215" alt="image" src="https://github.com/user-attachments/assets/1bb385d4-c079-46ce-8b6f-5b74a2628535" />


## Kesimpulan  
Hasil praktikum menunjukkan bahwa konfigurasi berhasil ketika seluruh perangkat dapat melakukan *ping* antar subnet tanpa error.
# Tampilan Topologi #
<img width="440" height="505" alt="image" src="https://github.com/user-attachments/assets/0b6384f0-4df6-4644-9b31-eb521fc2c6a6" />

