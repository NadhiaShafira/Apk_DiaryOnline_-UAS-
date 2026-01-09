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

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/854a04a6c71ddf9445e7a1936f5a4a8243ad960b/pict_projectUAS/dashboard_admin.png)

Session digunakan untuk menyimpan data login dan role pengguna.

**📌 Fitur Aplikasi (CRUD)**

**✍️ Create – Tulis Diary**

User dapat menulis diary dengan judul dan isi.

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/073e0611dcfc7f983f0143b10485c7a04e686c0b/pict_projectUAS/tulis_diary.png)

**📖 Read – Lihat Diary**

User dapat melihat daftar diary miliknya.

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/736ba14e43b6c379ac3eed9bad24545ca2a718f7/pict_projectUAS/catatan.png)

**✏️ Update – Edit Diary**

User dapat mengedit diary yang sudah dibuat.

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/a1c9a62e485531d8fb09f09d998cd0eaa0460fd1/pict_projectUAS/edit_diary.png)

**🗑️ Delete – Hapus Diary**

User dapat menghapus diary dengan konfirmasi.

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/df08c2233ece5e590650a594dce90135b5de75d5/pict_projectUAS/hapus_confirm.png)

**👑 Halaman Admin**

Admin memiliki halaman khusus untuk melihat seluruh diary dari semua user.

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/91e02ff9df9db7866d4e4cd251203f668cb99909/pict_projectUAS/admin_diary(1).png)

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/4391e58262c70461ab30d7de6b2441659f8efcb2/pict_projectUAS/admin_diary(2).png)

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

**📌 Fitur Pagination (User)**

**Deskripsi**

Pagination pada halaman Catatan Aku (User) digunakan untuk membatasi jumlah diary yang ditampilkan dalam satu halaman agar tampilan lebih rapi dan mudah dibaca.

Fitur ini dibuat menggunakan query MySQL LIMIT dan OFFSET.

**Cara Kerja**

Setiap halaman menampilkan 3 diary

Jika jumlah diary lebih dari 3, maka akan muncul nomor halaman

User hanya dapat melihat diary miliknya sendiri

Contoh Implementasi

Pagination diatur pada controller dengan perhitungan halaman dan offset, kemudian ditampilkan pada view catatan user.

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/444c71f8bda428badee1bff6df5dffa24fbfca23/pict_projectUAS/user_catatan_page1.png)

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/ae27acfcf09af08e0f7271d2cc7202db75562c0d/pict_projectUAS/user_catatan_page2.png)

![foto](https://github.com/NadhiaShafira/Apk_DiaryOnline_-UAS-/blob/fa3c5571e581bd9172d99b2fa931cf54fc4e1042/pict_projectUAS/user_catatan_page3.png)

**📌 Fitur Pagination (Admin)**

**Deskripsi**

Pagination pada halaman Admin – Semua Diary digunakan untuk menampilkan data diary dari seluruh user secara bertahap.
Fitur ini memudahkan admin dalam mengelola data diary tanpa menampilkan terlalu banyak data dalam satu halaman.

**Cara Kerja**

Admin dapat melihat semua diary dari seluruh user

Data ditampilkan per halaman menggunakan LIMIT dan OFFSET

Admin memiliki hak untuk melihat, mengedit, dan menghapus seluruh diary

Contoh Implementasi

Pagination diterapkan pada halaman admin dengan query yang mengambil seluruh data diary dari database.

![foto]()

![foto]()

**🧾 Kesimpulan**

Aplikasi Diary Online ini telah berhasil menerapkan sistem login dengan role admin dan user serta fitur CRUD menggunakan PHP dan MySQL sesuai dengan ketentuan UAS.

**❤️ Penutup**

Proyek ini dibuat untuk memenuhi tugas UAS Pemrograman Web dan diharapkan dapat menjadi dasar pengembangan aplikasi web sederhana.
