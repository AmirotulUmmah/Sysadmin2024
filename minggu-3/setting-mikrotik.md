### Pengaturan Koneksi Internet

Buat bridge1 sebagai bridge utama.
Aktifkan port ether 2 - 10.

##### NAT pada firewall:
![alt text](1?raw=true)
Action: masquerade
Chain: srcnat
Source Address: 192.168.1.0/24
Destination Address: 0.0.0.0/0
Out Interface: ether1

##### address list:
![alt text](?raw=true)
![alt text](?raw=true)
192.168.1.1/24 untuk 192.168.1.0 pada bridge1
192.168.88.1/24 untuk 192.168.88.0 pada ether1

Routing untuk terhubung ke internet:
0.0.0.0/0 ke 192.168.88.254 pada ether1
DNS server pada DHCP:
202.9.85.3
Melakukan penyesuaian IP dengan ipconfig /renew.


Pembuatan Jembatan (Bridge) dan Port:









![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
![alt text](?raw=true)
