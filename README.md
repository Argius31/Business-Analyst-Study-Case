# Flowchart-Supply
Flowchart for Supply Management
![Main Flowchart](https://github.com/Argius31/Business-Analyst-Study-Case/assets/122506192/796b39b9-e525-451b-8264-7357462966e2)

Main Flow
- User memasuki halaman utama pada aplikasi
- User memilih salah satu tombol pada interface yaitu tombol "login" atau "Register"
- Jika memilih "Login" akan dilanjutkan pada proses login
- jika memilih "Register" akan dilanjutkan pada proses register
- Jika tidak memilih apapun program selesai

Proses Login
- Setelah user memilih tombol login, user melakukan input email dan password
- Jika password tidak sesuai maka akan tampil "salah password" dan kembali ke melakukan input
- Jika sesuai maka login berhasil
- User dapat menggunakan fitur aplikasi dan melakukan submit tender proyek
- User bisa melanjutkan aktifitas pada aplikasi atau memilih logout
- Jika memilih logout akan kembali ke halaman utama

Proses Register
- Setelah user memilih tombol register, user melakukan input email, password dan nomor telepon
- Jika email sudah terdaftar maka akan tampil "Sudah terdaftar, silahkan login" dan diarahkan ke halaman utama untuk login
- Jika belum user akan menunggu proses approval dari manager logistik
- Jika tidak di approve oleh manager logistik akan kembali melakukan input
- Jika berhasil di approve oleh manager logistik maka akan tampil "Telah berhasil terdaftar"
- Jika user ingin login akan di arahkan kembali ke halaman utama

![ERD](https://github.com/Argius31/Business-Analyst-Study-Case/assets/122506192/b85ab211-361e-4f55-90da-9cfd9695a4e7)


Hubungan Antara Entitas:

Registrasi Perusahaan <-> Data Vendor: Hubungan one-to-many, di mana satu perusahaan dapat memiliki banyak data vendor terkait dengan bidang usaha dan jenis perusahaan yang berbeda.
Data Vendor <-> Status Persetujuan: Hubungan one-to-one, menunjukkan bahwa setiap data vendor memiliki satu status persetujuan yang terkait.

Registrasi Perusahaan:
- Pengguna memasukkan data perusahaan ke dalam aplikasi.
- Aplikasi memvalidasi dan menyimpan data perusahaan.

Proses Menjadi Vendor:
- Pengguna melengkapi data vendor (bidang usaha, jenis perusahaan).
- Aplikasi menyimpan data vendor yang terkait dengan perusahaan.
- Verifikasi dilakukan dan status persetujuan diberikan oleh manager logistik.

Persetujuan dan Status Vendor:
- Berdasarkan status persetujuan dari ERD, aplikasi menentukan apakah vendor diterima atau ditolak.
- Status persetujuan ditampilkan dalam antarmuka pengguna, menunjukkan keputusan terkait proses menjadi vendor.
