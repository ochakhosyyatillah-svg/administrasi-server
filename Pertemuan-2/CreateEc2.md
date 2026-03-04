# Membuat EC2 / Instance / VM

1. Pilih Menu All Services -> EC2
![alt text](image3.png)

2. di dalam menu EC kita pilih instance
![alt text](image4.png)

3. didalam menu instance pilih launch instance
![alt text](image5.png)

4. Beri nama Instance kita dengan format NIM_server
![alt text](image6.png)

5. kita pilih OS server untuk instance
![alt text](image7.png)

6. pilih Resource instance T3.Micro (2VCPU, 1GB Memory)
![alt text](image8.png)

7. membuat key pair, pilih new key pair, isi nama key, pilih RSA, format file.pem, create key pair
![alt text](image9.png)

8. Setting kebijakan keamanan/Security Group
   1. Allow SSH - Artinya membolehkan remote SSH dari luar
   2. Allow HTTPS - Artinya Instance bisa diakses dari protocol HTTPS
   3. Allow HTTP -> Artinya instance bisa di akses dari protocol HTTP
![alt text](image10.png)

9. selesai Set-up pilih Launch Instance
![alt text](image11.png)

10. Pastikan Launch Instance Sukses
![alt text](image12.png)
