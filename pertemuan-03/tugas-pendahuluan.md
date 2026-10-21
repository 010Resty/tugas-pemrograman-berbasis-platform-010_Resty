# Tugas Pendahuluan Pertemuan 3

## Identitas

| Keterangan | Isi |
|---|---|
| Nama | Resty Amylia Margareta |
| NIM | 2024520010 |
| Pertemuan | 3 |

## Soal 1 — Perbandingan Bootstrap dan Tailwind CSS
Bootstrap menggunakan class komponen seperti card, card-body, card-title, btn, dan btn-primary untuk membuat kartu dan tombol. Sementara itu, Tailwind CSS menggunakan class utility seperti bg-white, p-4, rounded-lg, shadow-md, dan text-blue-600 untuk mengatur tampilan secara langsung. Menurut saya, Bootstrap lebih mudah digunakan oleh pemula karena menyediakan komponen siap pakai sehingga tidak perlu menyusun banyak class utility dari awal.

## Soal 2 — Rancangan Kartu Biodata dengan Dua Pendekatan

# Sketsa Kartu Biodata
<img width="260" height="193" alt="image" src="https://github.com/user-attachments/assets/5fdfd70b-77e0-45df-b1ed-08f15a5b0959" />


# A. Versi komponen (Bootstrap)
<div class="card" style="width: 18rem;">
  <img src="foto.jpg" class="card-img-top" alt="Foto mahasiswa">
  <div class="card-body">
    <h5 class="card-title">Resty Amylia Margareta</h5>
    <p class="card-text">NIM: 2024520010</p>
    <a href="#" class="btn btn-primary">Lihat Biodata</a>
  </div>
</div>

Jumlah aturan CSS tambahan yang perlu ditulis: 0 aturan, jika menggunakan komponen bawaan Bootstrap tanpa modifikasi.

# B. Versi utility (Tailwind CSS)
<div class="w-72 rounded-lg bg-white shadow-md overflow-hidden">
  <img src="foto.jpg" class="w-full h-48 object-cover" alt="Foto mahasiswa">
  <div class="p-4">
    <h5 class="text-lg font-bold">Resty Amylia Margareta</h5>
    <p class="mt-2 text-gray-600">NIM: 2024520010</p>
    <a href="#" class="mt-4 inline-block rounded bg-blue-600 px-4 py-2 text-white">
      Lihat Biodata
    </a>
  </div>
</div>

Jumlah class utility: 19 kemunculan class jika setiap nama class pada atribut class dihitung satu per satu, termasuk class yang dipisahkan spasi.

Kesimpulannya, versi utility Tailwind lebih mudah diubah warnanya secara langsung melalui class seperti bg-blue-600, sedangkan Bootstrap lebih praktis untuk tampilan standar tetapi biasanya membutuhkan penggantian class atau CSS tambahan untuk penyesuaian khusus.

 ## Soal 3 — Mengamati Isi Token JWT
Token JWT terdiri dari 3 bagian, yaitu header, payload, dan signature, yang dipisahkan oleh tanda titik (.). Pada payload token yang diberikan, terdapat tiga nama data, yaitu sub, name, dan iat, yang masing-masing menunjukkan identitas subjek, nama pengguna, dan waktu penerbitan token. Password tidak boleh disimpan di dalam payload JWT karena isi payload dapat dibaca setelah didekodekan dan tidak otomatis terenkripsi, sehingga password dapat diketahui oleh pihak yang tidak berwenang.

## Soal 4 — Analogi Gerbang Kampus
Pemeriksaan di gerbang UNIRA merupakan contoh authentication, yaitu proses memastikan identitas seseorang melalui kartu mahasiswa atau identitas lainnya. Sementara itu, pemeriksaan di depan ruang server merupakan contoh authorization, yaitu proses menentukan apakah orang tersebut memiliki izin untuk memasuki ruangan berdasarkan perannya. Contohnya, mahasiswa berhasil menunjukkan kartu mahasiswa yang valid, tetapi tetap tidak diizinkan masuk ke ruang server karena hanya teknisi laboratorium yang memiliki akses.

## Soal 5 — Peran dalam Aplikasi Nyata
Aplikasi yang dipilih adalah GitHub. Tiga contoh peran di dalam repositori GitHub adalah owner yang memiliki kendali penuh atas repositori, maintainer yang mengelola pemeliharaan proyek sesuai izin yang diberikan, dan collaborator yang berkontribusi pada proyek sesuai tingkat aksesnya; salah satu fitur yang dibatasi adalah penghapusan repositori, yang hanya dapat dilakukan oleh pemilik atau pihak yang memiliki izin administratif yang sesuai.
