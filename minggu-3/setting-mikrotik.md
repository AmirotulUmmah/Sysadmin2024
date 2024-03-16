# Setting Mikrotik

Buat bridge1 sebagai bridge utama. <br>
Aktifkan port ether 2 - 10.

### NAT pada firewall:
![alt text](https://github.com/AmirotulUmmah/Sysadmin2024/blob/main/minggu-3/assets/1.jpeg?raw=true) <br>
* Action: masquerade
* Chain: srcnat
* Source Address: 192.168.1.0/24
* Destination Address: 0.0.0.0/0
* Out Interface: ether1<br>

### Address list
* Tambahkan Route untuk Ether1 : 0.0.0.0/0 192.168.88.254 ether1 <br>
![alt text](https://github.com/AmirotulUmmah/Sysadmin2024/blob/main/minggu-3/assets/2.jpeg?raw=true)<br><br>

* 192.168.1.1/24 untuk 192.168.1.0 pada bridge1
* 192.168.88.1/24 untuk 192.168.88.0 pada ether1
![alt text](https://github.com/AmirotulUmmah/Sysadmin2024/blob/main/minggu-3/assets/3.jpeg?raw=true)


### Routing untuk terhubung ke internet
![alt text](https://github.com/AmirotulUmmah/Sysadmin2024/blob/main/minggu-3/assets/4.jpeg?raw=true)<br><br>

* DNS server pada DHCP: 202.9.85.3
  
![alt text](https://github.com/AmirotulUmmah/Sysadmin2024/blob/main/minggu-3/assets/5.jpeg?raw=true)<br>
