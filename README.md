# Jarkom-Modul-4-ITB05-2022
Kelompok ITB05

1. M.Fernando N.Sibarani (5027201015)
2. Richard Nicolas (5027201021)
3. Muhammad Ihsanul Afkar (5027201024)

# Daftar Isi
* [Topologi](#Topologi)
* [VLSM](#VLSM) 
* [Revisi_VLSM](#RevisiVLSM)
* [CIDR](#CIDR) 
* [kendala](#Kendala) 

# Topologi
Berikut ini adalah topologi dari soal yang akan kami buat di **Cicso Packet Tracer** dan **GNS3**
![topologi](img/topologi.png)
# VLSM
Untuk topologi VLSM, kami menggunakan **Cisco Packet Tracer** dalam pembuatan topologi
Berikut ini adalah topologi pada Cicso Packet Tracer
![topologi](img/topologi_vlsm.png)

Berikut ini adalah tabel subnetting VLSM yang kami lakukan
![tabel](img/tabel_vlsm.png)

Berikut ini adalah subnetting VLSM tree yang kami buat
![tree](img/vlsm_tree.png)

Step pengerjaan:
Pada setiap node, kami mengatur **IP address**, **subnet mask**, dan **default gateway** (IP address dan subnet mask diatur berdasarkan tabel VLSM, default gateway adalah IP dari router yang terhubung dengan node)

Contoh salah satu pengaturan adalah pada Guideau yang memiliki 1000 host (A1)
![cpt1](img/cpt1.png)
Setelah itu, diatur pada router IP address untuk semua jalur yang terhubung dengan router tersebut (A1 menggunakan FastEthernet0/0)

![cpt2](img/cpt2.png)

(A4 menggunakan FastEthernet0/1)

![cpt2.2](img/cpt2_2.png)

(A8 menggunakan FastEthernet1/0

![cpt2.3](img/cpt2_3.png)

Setelah FastEthernet diatur, maka pada bagian **ROUTING** > **Static** diatur Network, Mask, dan Next Hop 

Untuk memudahkan pengerjaan, kami menggaunakan **0.0.0.0** pada **network** dan **mask**, dan untuk **Next hop** digunakan **ip router yang terhubung**. Contohnya pada **The Dauntless** terhubung dengan IP **The Minister** (IP Router)
![cpt3](img/cpt3.png)


## Revisi VLSM
ping dari The Dauntless ke The Profound

![cptdp](img/cpt_dp.png)

ping dari The Witch ke The Order

![cptwo](img/cpt_wo.png)

ping dari Guideau ke The Firefist (masih tidak bisa)

![cptgf](img/cpt_gf.png)

# CIDR
Berikut ini adalah topologi pada GNS3
![topologi](img/topologi_cidr.png)

Berikut ini adalah tabel subnetting CIDR yang kami lakukan
![tabel](img/tabel_cidr.png)

Step subnetting CIDR
![step1](img/CIDR1.png)
![step2](img/CIDR2.png)
![step3](img/CIDR3.png)
![step4](img/CIDR4.png)
![step5](img/CIDR5.png)
![step6](img/CIDR6.png)
![step7](img/CIDR7.png)
![step8](img/CIDR8.png)

Berikut ini adalah subnetting CIDR tree yang kami buat
![tree](img/cidr_tree.png)

Pada GNS3, berikut ini adalah topologi yang dibuat
![gns](img/gns1.png)

Terdapat kendala sehingga masih tidak bisa nge-*ping* node lain 

![gns](img/gns2.png)

# Kendala
CIDR pada GNS3 terdapat kendala sehingga masih tidak bisa nge-*ping* antara pc dengan pc ataupun router dengan router