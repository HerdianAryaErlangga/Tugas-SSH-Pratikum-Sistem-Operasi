## Informasi Mahasiswa
**Nama: Herdian Arya Erlangga**\
**NIM: 09011182328099**\
**Kelas: SK3C**
<br>
<div align="Center">
  
## INSTALL AND CONFIGURATION SSH

</div>

### Prepare Ubuntu
Langkah pertama yang perlu dilakukan adalah mempersiapkan Ubuntu dengan cara:
  - > sudo apt update && apt upgarade

    ![Update & Upgrade](https://github.com/user-attachments/assets/4de06745-0df9-4d00-b6e4-20e11fdd07a9)


<br>

### Install SSH on Ubuntu
Selanjutnya lakukan penginstallan SSH di Ubuntu, disini saya menggunakan Ubuntu 22.04 
  - > sudo apt install openssh-server

    ![Install SSH](https://github.com/user-attachments/assets/92a7ac19-b0a5-426e-a459-09d4eec32538)


<br>

### Start SSH
Mulai program SSh
  - > sudo systemctl enable --now ssh

    ![Enable SSH](https://github.com/user-attachments/assets/244aabd4-e587-4d6c-9e10-ae772d38352a)


Cek status
  - > sudo systemctl status ssh
    
    ![Cek Status SSH](https://github.com/user-attachments/assets/f0fc4d06-f5c7-4f24-bfe1-5de9574bed2b)


<br>

### Configuration The Firewall
Cek UFW status
  - > sudo ufw status

    ![Cek Firewall Status](https://github.com/user-attachments/assets/480f9488-ca09-408a-9b24-5705336e6efd)


Jika status UFW inactive seperti di kasus ini, maka kita dapat mengaktifkan dengan:
  - > sudo ufw enable
     
    ![Enable Firewall](https://github.com/user-attachments/assets/d418a14e-d420-44a9-a24f-cd57c638c830)

Selanjutnya izinkan lalu lintas SSH
  - > sudo ufw allow ssh
    
    ![Allow SSH](https://github.com/user-attachments/assets/33600e37-6424-48d7-96a4-dd8d3a2e711d)


<br>

### Connect to The Server
Sambungkan ke server sendiri dengan user dan ip sendiri
  - > ssh anggaa17@192.168.49.129

    ![Connect Ke anggaa17](https://github.com/user-attachments/assets/811316d5-73e2-4977-863d-e7db924ea042)

Mencoba untuk connect ke SSH server sendiri melalui Putty dan CMD
  - > Connect Dari Putty

    ![Putty](https://github.com/user-attachments/assets/3198d703-bdee-478a-8aa8-5242045fcbab)

  - > Connect Dari CMD

    ![CMD](https://github.com/user-attachments/assets/b53809f1-624d-4c80-b8cd-ad616136de0b)


Selanjutnya coba untuk menghubungkan kepada komputer lain dengan user mereka dan ip mereka, pastikan dalam satu jaringan yang sama:
  - > ssh syf@192.168.49.179

    ![YZcP8bz3lI](https://github.com/user-attachments/assets/66cd88eb-ab2b-425a-b9fd-a6e7a89f4a87)
    ![RQz31CdnIV](https://github.com/user-attachments/assets/86ba1b68-2945-4890-b1c0-3ec05add89d7)
