# Laporan Hasil Praktikum: Final Project Aplikasi Berbasis Container

## Identitas Mahasiswa

- **Nama:** Made Wahyu Dharmayoga
- **NIM:** 2415354010
- **Kelas/Rombel:** TRPL B
- **Tanggal Praktikum:** 20 Mei 2026

---

## Teknologi & Tools yang Digunakan

- **Sistem Operasi:** Windows 11
- **Containerization:** Docker & Docker Hub
- **Bahasa Pemrograman / Framework:** Node.js
- **Tools Lain:** VS Code, Git, Hoppscotch

---

## Langkah-Langkah Praktikum & Dokumentasi

---

### Langkah 1: Membuat Struktur Projek

Membuat struktur folder untuk projek.

**Dokumentasi/Screenshot:**

<img width="146" height="180" alt="image" src="https://github.com/user-attachments/assets/9d25ff04-47c8-42c7-b01f-c7fa2f53b250" />

---

### Langkah 2: Mengisi File Dockerfile, app.js, docker-compose.yml

Membuat isi dari file-file tersebut berdasarkan dari projek latihan sebelumnya. pada app.js ditambahkan dengan kode untuk put dan delete.

**Dokumentasi/Screenshot:**

<img width="251" height="153" alt="image" src="https://github.com/user-attachments/assets/8229f36d-9bcd-47cd-8bdf-bc362b8f91e5" />

---

### Langkah 3: Menjalankan Docker Compose

```bash
docker compose up -d --build
```

**Dokumentasi/Screenshot:**

<img width="776" height="161" alt="image" src="https://github.com/user-attachments/assets/715b2ba0-eada-47cc-9d06-e3ebb7622347" />

### Langkah 4: Melakukan Pengujian Compose, Volume, Container, Network

**Pengujian Volume**
```bash
docker volume ls
```

**Pengujian Container**
```bash
docker ps
```

**Pengujian Network**
```bash
docker exec -it container-final sh
ping mysql-db
```

**Dokumentasi/Screenshot:**

  **Pengujian Compose**

  <img width="792" height="167" alt="image" src="https://github.com/user-attachments/assets/0cf35c65-d70b-4023-9b68-73e54c078a5a" />

  **Pengujian Volume**

  <img width="244" height="46" alt="image" src="https://github.com/user-attachments/assets/5e6804ec-c137-411d-a8ff-a298deaf832e" />  

  **Pengujian Container**

  <img width="965" height="70" alt="image" src="https://github.com/user-attachments/assets/dcb2f2e8-502f-4867-8cc3-d2813fb226be" />  

  **Pengujian Network**

  <img width="749" height="209" alt="image" src="https://github.com/user-attachments/assets/709615b1-a398-45fa-bdab-8c2e0e5911c9" />

---

### Langkah 5: Melakukan Pengujian di Browser

Jelaskan bagaimana cara melakukan verifikasi atau pengujian bahwa praktikum Anda berhasil berjalan.

**Dokumentasi/Screenshot:**

<img width="405" height="192" alt="image" src="https://github.com/user-attachments/assets/48c59c23-2ef3-4460-8ccb-df49c343ba25" />

---

### Langkah 6: Melakukan Pengujian di Hoppscotch

Melakukan pengujian di Hoppscotch. Berikan link http://localhost:3000/ pada Hoppscotch. Untuk pengujian get kita hanya perlu untuk memilih 'GET' dan klik pada kirim untuk melihat semua user. Untuk insert ganti dengan memilih pada 'POST', pada bagian body ganti dengan 
content type application/json lalu berikan value baru pada 'name'. Untuk update pilih 'PUT' dan akhiran linknya diganti dengan users/[id] sesuai dengan id yang ingin diupdate. Untuk delete pilih 'DELETE' dengan link berakhiran users/[id] id sesuai dengan id yang ingin dihapus.

**Dokumentasi/Screenshot:**

**Pengujian Get**

<img width="1308" height="656" alt="image" src="https://github.com/user-attachments/assets/7cb70eb8-c41c-4c09-9052-6ba03ebe08dd" />

**Pengujian Post**

<img width="1321" height="559" alt="image" src="https://github.com/user-attachments/assets/f40fdbd5-5eb2-4591-9a3c-7fc86bef7e3d" />

**Pengujian Put**

<img width="1187" height="563" alt="image" src="https://github.com/user-attachments/assets/ff112f7d-8039-4858-b90e-ec54e7c8023a" />

**Pengujian Delete**

<img width="1175" height="590" alt="image" src="https://github.com/user-attachments/assets/51267c20-9807-448d-92a3-1d41aa1b433b" />

---

### Langkah 7: Melakukan Push ke Docker

Melakukan push image ke docker.

```bash
docker tag image-final derisstrict/image-final
docker push derisstrict/image-final
```

### Langkah 8: Menambahkan Repository Github

Pada github desktop, pada menu File > New repository. Tambahkan nama repository dan path ke projeknya.

**Dokumentasi/Screenshot:**

<img width="954" height="655" alt="image" src="https://github.com/user-attachments/assets/a7d68b3e-f9df-43d8-9bf1-726c608a5227" />

## Kesimpulan

Kendala yang dialami adalah database awalnya tidak terkoneksi karena salahnya nama database.
