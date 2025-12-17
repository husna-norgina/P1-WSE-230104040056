# 🌐 Praktikum — Demo Testing API (Postman)

Praktikum ini membahas **pengujian Web Service (API)** menggunakan **Postman** dengan memanfaatkan **JSONPlaceholder**, yaitu API publik (dummy API) yang digunakan untuk simulasi proses komunikasi client–server. Praktikum ini mencakup pengujian metode HTTP **GET, POST, PUT, dan DELETE** serta pemahaman konsep request–response berbasis **JSON**.

**Topik:** Demo Testing API (HTTP Method & REST API)

---

## 🧑‍🎓 Informasi Mahasiswa

| Informasi          | Data                                                       |
|--------------------|------------------------------------------------------------|
| Mata Kuliah        | Web Service Engineering                                    |
| Dosen Pengampu     | Muhayat, M.IT                                              |
| Praktikum / Proyek | P1 – Demo Testing API                                      |
| Nama Mahasiswa     | Husna Norgina                                              |
| NIM                | 230104040056                                               |
| Kelas              | TI23B                                                      |
| Repo GitHub        | https://github.com/husna-norgina/P1-WSE-230104040056       |
| Tanggal Praktikum  | 17-11-2025                                                 |

---

## 🎯 Tujuan Praktikum

1. Memahami konsep dasar Web Service dan REST API.
2. Mengetahui fungsi dan perbedaan metode HTTP (GET, POST, PUT, DELETE).
3. Melakukan pengujian endpoint API menggunakan Postman.
4. Memahami struktur request dan response dalam format JSON.
5. Melatih kemampuan analisis hasil pengujian API.

---

## 🛠 Tools & Environment

### **Tools yang Digunakan**

- Postman (Desktop / Web)
- JSONPlaceholder (Public Dummy API)
- GitHub (Repository Dokumentasi)

---

## 🌍 API yang Digunakan

**JSONPlaceholder**  
Merupakan API publik gratis yang digunakan untuk simulasi pembelajaran REST API.

**Base URL:**
```

https://jsonplaceholder.typicode.com

````

---

## 🔁 Metode HTTP yang Diuji

### 🔵 1. GET — Ambil Semua Data Post

| Method | Endpoint | Keterangan                     |
| ------ | -------- | ------------------------------ |
| GET    | `/posts` | Mengambil seluruh data posting |

**Hasil:**  
![alt text](<1. GET All Posts.png>)
Menampilkan daftar posting dalam bentuk JSON array.
Server merespons status `200 OK`.

---

### 🔵 2. GET — Ambil Data Berdasarkan ID

| Method | Endpoint   | Keterangan                              |
| ------ | ---------- | --------------------------------------- |
| GET    | `/posts/1` | Mengambil satu data post berdasarkan ID |

**Hasil:**  
![alt text](<2. GET Post by ID.png>)
Menampilkan satu objek JSON dengan ID tertentu.
Server merespons status `200 OK`.

---

### 🔵 3. GET — Query Parameter

| Method | Endpoint             | Keterangan                             |
| ------ | -------------------- | -------------------------------------- |
| GET    | `/comments?postId=1` | Mengambil komentar berdasarkan ID post |

**Hasil:**  
![alt text](<3. GET Comments by postId.png>)
Menampilkan daftar komentar dengan `postId = 1`.
Server merespons status `200 OK`.

---

### 🟢 4. POST — Menambahkan Data Baru

| Method | Endpoint | Keterangan                 |
| ------ | -------- | -------------------------- |
| POST   | `/posts` | Menambahkan data post baru |

**Body (JSON):**
```json
{
  "title": "Belajar API",
  "body": "Ini percobaan pertama",
  "userId": 1
}
````

**Hasil:**
![alt text](<4. POST Create Post.png>)
Server merespons data baru dengan ID tambahan (simulasi).
Server merespons status `201 Created`.

---

### 🟡 5. PUT — Mengubah Data

| Method | Endpoint   | Keterangan                        |
| ------ | ---------- | --------------------------------- |
| PUT    | `/posts/1` | Mengubah data post berdasarkan ID |

**Body (JSON):**

```json
{
  "id": 1,
  "title": "Belajar API Update",
  "body": "Isi sudah diperbarui",
  "userId": 1
}
```

**Hasil:**
![alt text](<5. PUT Update Post.png>)
Data berhasil diperbarui (simulasi).
Server merespons status `200 OK`.

---

### 🔴 6. DELETE — Menghapus Data

| Method | Endpoint   | Keterangan                         |
| ------ | ---------- | ---------------------------------- |
| DELETE | `/posts/1` | Menghapus data post berdasarkan ID |

**Hasil:**
![alt text](<6. DELETE Post.png>)
Menghapus data berdasarkan `postId = 1`.
Server merespons status `200 OK`.

---

### 📄 7. Laporan Praktikum 1
[230104040056_Husna Norgina_P1](<evidence/230104040056_Husna Norgina_P1.pdf>)

---

> Semua hasil uji Postman dan laporan praktikum 1 disimpan di folder: `./evidence/`

---

## 📊 Analisis Praktikum

* Metode **GET** berhasil menampilkan data sesuai endpoint yang diakses.
* Metode **POST** berhasil mensimulasikan penambahan data baru.
* Metode **PUT** berhasil memperbarui data yang ada.
* Metode **DELETE** berhasil menghapus data secara simulatif.
* Semua komunikasi data menggunakan format **JSON**.
* Postman sangat membantu dalam pengujian dan analisis Web Service.

---

## ✅ Kesimpulan

Berdasarkan praktikum yang telah dilakukan, dapat disimpulkan bahwa pengujian Web Service menggunakan Postman berjalan dengan baik. Setiap metode HTTP (GET, POST, PUT, dan DELETE) berfungsi sesuai dengan konsep REST API. JSONPlaceholder sebagai API dummy sangat efektif digunakan sebagai media pembelajaran untuk memahami mekanisme request–response antara client dan server. Praktikum ini memberikan pemahaman dasar yang kuat mengenai pengujian API dalam pengembangan sistem berbasis web service.

---

## 📌 Catatan

* Semua pengujian dilakukan menggunakan Postman.
* API yang digunakan bersifat dummy (simulasi).
* Data tidak benar-benar tersimpan di server.

---
📝 *Disusun oleh Husna Norgina (230104040056) — Praktikum 1 Web Service Engineering*
