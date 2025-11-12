# **Praktikum Jaringan komputer**

# *Tugas Akhir 3 Configure VLANs and Trunking*

## Video Demonstrasi  
[🔗 Klik di sini untuk menonton video praktikum di YouTube](https://youtu.be/39BDp6FA05I)


## File Cisco Packet Tracer  
**TA 3** `TA3.pkt`  
[Klik di sini untuk mengunduh file Cisco Packet Tracer](Judul%203.pkt)

## Topologi Jaringan  
Berikut adalah tampilan topologi jaringan yang digunakan pada praktikum ini:

## Deskripsi Singkat  
Lab Packet Tracer ini mengonfigurasi VLAN dan 802.1Q Trunking untuk meningkatkan performa dan keamanan jaringan. Dimulai dengan membuat VLAN terpisah (seperti VLAN 10 untuk "Operations" dan VLAN 99 untuk "Management") dan mendaftarkan port PC serta SVI switch ke VLAN tersebut.

## Hasil Pengujian Akhir (Setelah Trunking Dikonfigurasi)
Tabel ini merangkum hasil konektivitas akhir dari lab setelah S1 dan S2 terhubung melalui link trunk 802.1Q.
| Dari (Sumber) | Ke (Tujuan) | VLAN Sumber | VLAN Tujuan | Status Ping | Alasan |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **PC-A** | **PC-B** | VLAN 10 | VLAN 10 | ✅ **BERHASIL** | Perangkat berada di VLAN yang sama, dan trunk mengizinkan lalu lintas VLAN 10. |
| **S1** | **S2** | VLAN 99 | VLAN 99 | ✅ **BERHASIL** | Perangkat berada di VLAN yang sama (Management), dan trunk mengizinkan lalu lintas VLAN 99. |
| **PC-A** | **S1** | VLAN 10 | VLAN 99 | ❌ **GAGAL** | Perangkat berada di VLAN yang berbeda. Diperlukan router (Layer 3) untuk Inter-VLAN routing. |
| **PC-B** | **S2** | VLAN 10 | VLAN 99 | ❌ **GAGAL** | Perangkat berada di VLAN yang berbeda. Diperlukan router (Layer 3) untuk Inter-VLAN routing. |

## Kesimpulan  
Lab ini menunjukkan bahwa VLAN berhasil memisahkan jaringan ke dalam grup yang berbeda (seperti VLAN 10 dan 99) . Pemisahan ini awalnya memutus komunikasi antar PC di switch yang berbeda. Masalah ini diatasi dengan mengonfigurasi 802.1Q Trunk , yaitu jalur khusus yang memungkinkan lalu lintas dari berbagai VLAN (VLAN 10 dan 99) lewat di antara switch. Hasil akhirnya, komunikasi di dalam VLAN yang sama (PC-A ke PC-B) berhasil dipulihkan , sementara komunikasi antar VLAN yang berbeda (PC-A ke S1) tetap terisolasi.

