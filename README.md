# Otomasi Manajemen Rule-set Suricata IDS Berbasis CI/CD Pipeline Jenkins

Project akhir ini mengintegrasikan **Suricata IDS** dengan **ELK Stack** untuk sistem pemantauan keamanan jaringan yang terpusat.

## Arsitektur Sistem
- **Sensor (PC-6)**: Ubuntu Server, Suricata IDS, Filebeat.
- **Server Pusat**: Elasticsearch & Kibana (IP 192.168.4.9).

## Cara Penggunaan
1. Salin file di folder `config/` ke direktori `/etc/` masing-masing layanan.
2. Restart layanan: `sudo systemctl restart suricata filebeat`.

## Hasil Pengujian
Sistem berhasil mendeteksi simulasi serangan `curl http://testmyids.com` dan menampilkannya di dashboard Kibana.
