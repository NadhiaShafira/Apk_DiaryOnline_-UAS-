# Apk_DiaryOnline_-UAS-

**Nama                 : Nadhia Shafira_312410498**

**Kelas                : TI.24.A.5**

**Matkul               : Pemograman Web 1**

**Dosen Pengampu       : Agung Nugroho, S.Kom., M.Kom.**

---

**📝 Deskripsi Proyek**

Aplikasi Diary Online adalah aplikasi web berbasis PHP dan MySQL yang digunakan untuk mencatat diary harian secara digital.
Aplikasi ini dibuat untuk memenuhi tugas Ujian Akhir Semester (UAS) Pemrograman Web dengan menerapkan konsep CRUD, OOP, Session, dan Role Admin & User.

**🎯 Tujuan Pembuatan**

1. Menerapkan pemrograman web menggunakan PHP & MySQL

2. Mengimplementasikan sistem login dengan role admin dan user

3. Mengimplementasikan fitur CRUD (Create, Read, Update, Delete)

4. Menggunakan konsep Object Oriented Programming (OOP)

**🛠️ Teknologi yang Digunakan**

1. PHP

2. MySQL

3. HTML

4. CSS

5. Apache (XAMPP)

**📂 Struktur Folder**

diary_gemes/
├── app/

│   ├── controllers/

│   │   ├── AuthController.php

│   │   └── DiaryController.php

│   └── views/

│       ├── login.php

│       ├── dashboard.php

│       ├── tulis.php

│       ├── catatan.php

│       ├── edit.php

│       └── admin_diary.php

├── config/

│   └── Database.php

├── public/

│   └── css/

│       └── style.css

├── screenshots/

├── index.php

└── README.md

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/3d1c872f2d916233bebca47fe4af6411018e098f/pict_projectUAS/struktur_folder.png)

**🗄️ Database**

_Nama database: diary_db_

Tabel users

| Field    | Keterangan    |
| -------- | ------------- |
| id       | Primary Key   |
| nama     | Nama pengguna |
| email    | Email         |
| password | Password      |
| role     | admin / user  |

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/2c2e75abe434968ccbdcc203273da82f007ffa37/pict_projectUAS/database_users.png)

Tabel diary

| Field   | Keterangan  |
| ------- | ----------- |
| id      | Primary Key |
| user_id | Relasi user |
| judul   | Judul diary |
| isi     | Isi diary   |
| tanggal | Tanggal     |

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/4805b5e451465a6a7bbf4c245457ec049685edfb/pict_projectUAS/database_diary.png)

**🔐 Sistem Login & Role**

_Tampilan Saat Login_

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/3a85c722d8033f9358ccacb3f839815f9a002a58/pict_projectUAS/login.png)

Aplikasi memiliki dua role:

1. User → menulis, melihat, mengedit, dan menghapus diary pribadi

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/540570389bc2412c529b065698c25d288fb04056/pict_projectUAS/dashboard_user.png)

2. Admin → melihat seluruh diary dari semua user

![foto]()

Session digunakan untuk menyimpan data login dan role pengguna.

**📌 Fitur Aplikasi (CRUD)**

**✍️ Create – Tulis Diary**

User dapat menulis diary dengan judul dan isi.

![foto]()

**📖 Read – Lihat Diary**

User dapat melihat daftar diary miliknya.

![foto]()

**✏️ Update – Edit Diary**

User dapat mengedit diary yang sudah dibuat.

![foto]()

**🗑️ Delete – Hapus Diary**

User dapat menghapus diary dengan konfirmasi.

![foto]()

**👑 Halaman Admin**

Admin memiliki halaman khusus untuk melihat seluruh diary dari semua user.

![foto]()

![foto]()

**🧪 Pengujian**

Aplikasi diuji menggunakan metode black box.

| Fitur             | Status    |
| ----------------- | --------- |
| Login             | Berhasil  |
| Session           | Berjalan  |
| CRUD              | Berhasil  |
| Role Admin & User | Berfungsi |
| Logout            | Berhasil  |

**🚀 Cara Menjalankan Aplikasi**

1. Jalankan Apache & MySQL pada XAMPP

2. Simpan folder project di htdocs

3. Import database diary_db

4. Akses melalui browser:

```http://localhost/diary_gemes/login
```

**📌 Akun Uji Coba**

_Admin_

Email    : admin@gmail.com
Password : 12345

_User_

Email    : user@gmail.com
Password : 12345
Nama     : User Cantik


**🧾 Kesimpulan**

Aplikasi Diary Online ini telah berhasil menerapkan sistem login dengan role admin dan user serta fitur CRUD menggunakan PHP dan MySQL sesuai dengan ketentuan UAS.

**❤️ Penutup**

Proyek ini dibuat untuk memenuhi tugas UAS Pemrograman Web dan diharapkan dapat menjadi dasar pengembangan aplikasi web sederhana.
