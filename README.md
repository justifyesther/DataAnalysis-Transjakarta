# `PROYEK AKHIR MODUL 2 - TRANSAKSI TRANSPORTASI UMUM TRANSJAKARTA -`

**OLEH: JUSTIFY ESTER PASARIBU (JCDS 0406 006)**

**Berdasarkan Dataset dari Kaggle yang dapat Diaskes [disini](https://www.kaggle.com/datasets/dikisahkan/transjakarta-transportation-transaction/data), untuk memahami lebih dalam mengenai dataset Public Transportation Transaction Transjakarta. Berikut ini Pemahaman Dasar dari Dataset :**

> **TENTANG DATASET**

Dataset ini adalah simulasi data transaksi Transjakarta, dibuat untuk memfasilitasi analisis dan pengembangan model data. Setiap transaksi memiliki ID unik, informasi kartu pembayaran termasuk bank penerbit, nama pemegang, jenis kelamin, dan tanggal lahir pemegang kartu. Data juga mencakup ID koridor, nama koridor, arah rute, informasi pemberhentian (termasuk garis lintang dan bujur), urutan pemberhentian, waktu tap-in dan tap-out, serta jumlah pembayaran.

> **KONTEKS**

Transjakarta adalah perusahaan transportasi umum di Jakarta, Indonesia, menggunakan bus besar, bus sedang, dan bus mini. Sistem pembayaran menggunakan kartu tap-in dan tap-out. Dataset ini tidak mewakili data transaksi nyata Transjakarta tetapi memberikan kerangka untuk analisis model transportasi umum.

> **KONTEN**

Dataset ini menyediakan informasi terperinci tentang transaksi simulasi, mencakup aspek-aspek seperti rute, waktu perjalanan, dan biaya. Ini berguna untuk menganalisis pola perjalanan penumpang dan efisiensi rute.

> **INSPIRASI**

Dataset ini dapat digunakan untuk memahami dinamika transportasi umum di Jakarta. Analisis ini dapat membantu mengidentifikasi rute yang sibuk, potensi kemacetan, dan preferensi penumpang, serta mendukung perencanaan rute yang lebih efisien.

# `PEMANGKU KEPENTINGAN: Divisi Manajemen Operasional TransJakarta`

Memilih Divisi Manajemen Operasional Transjakarta sebagai pemangku kepentingan yang tepat berdasarkan dataset Transjakarta adalah pilihan yang sesuai karena:

- **Relevansi Data:** Dataset ini menyediakan informasi mendetail tentang transaksi perjalanan yang sangat berguna untuk manajemen operasional.
- **Fokus pada Operasional:** Divisi ini berfokus pada pengelolaan operasi sehari-hari, efisiensi rute, dan peningkatan kualitas layanan, yang semua aspeknya dapat dianalisis menggunakan dataset Transjakarta.

# `LATAR BELAKANG`

Manajemen Operasional Transjakarta menghadapi tantangan dalam mengoptimalkan operasi dan meningkatkan layanan bagi penumpang. Efisiensi rute, waktu tunggu, kepadatan penumpang, dan pendapatan adalah beberapa area kunci yang membutuhkan perhatian. Dataset Transjakarta menyediakan data transaksi yang dapat digunakan untuk menganalisis aspek-aspek ini dan memberikan wawasan untuk peningkatan layanan.

# `PERNYATAAN MASALAH`

Divisi Manajemen Operasional Transjakarta menghadapi tantangan dalam memahami **bagaimana pola pergerakan penumpang dan faktor-faktor yang mempengaruhinya** untuk meningkatkan efisiensi layanan dan kepuasan pelanggan. Mereka perlu mengoptimalkan jadwal, mengatur alokasi sumber daya, dan mengidentifikasi area untuk peningkatan layanan.

Sebagai seorang analis data akan mencoba menjawab pertanyaan berikut:

**Bagaimana kita dapat menggunakan analisis data untuk memahami dan mengoptimalkan pola pergerakan penumpang dan kepadatan rute demi meningkatkan efisiensi operasional Transjakarta?**

---
Berdasarkan pernyataan masalah yang dijelaskan di atas, berikut ini adalah pertanyaan-pertanyaan yang akurat sesuai dengan pernyataan masalah tersebut:

**1. Bagaimana pola pergerakan penumpang di berbagai rute?**
- Justifikasi: Memahami pola ini akan membantu dalam menyesuaikan jadwal dan rute untuk mengurangi waktu tunggu dan penumpukan penumpang.
- Kolom Relevan: waktu masuk, waktu keluar, nama koridor, arah.
- Bantuan Analis Data: Menganalisis waktu dan frekuensi perjalanan untuk mengidentifikasi rute yang sibuk.

> ### **Informasi Terkait Variabel/Kolom pada Dataset**

Dataset ini berisi informasi tentang Transaksi Transportasi Umum Transjakarta. Untuk mengetahui lebih lanjut tentang dataset Transaksi Transportasi Umum Transjakarta, Anda dapat melihatnya [di sini](https://drive.google.com/drive/folders/1S04hk5uHfHYe6J1S6fVqDunuja1Lk1Lo). Terdapat 22 kolom dalam dataset `Transjakarta.csv`. Berikut ini adalah penjelasan dari setiap kolomnya:

1. `transID:` ID transaksi yang unik untuk setiap transaksi.
2. `payCardID:` Pengidentifikasi utama pelanggan, yaitu kartu yang digunakan sebagai tiket masuk dan keluar.
3. `payCardBank:` Nama bank penerbit kartu pelanggan.
4. `payCardName:` Nama pelanggan yang tertulis di kartu.
5. `payCardSex:` Jenis kelamin pelanggan yang tertulis di kartu.
6. `payCardBirthDate:` Tanggal lahir pelanggan.
7. `corridorID:` ID Koridor atau ID Rute sebagai kunci untuk pengelompokan rute.
8. `corridorName:` Nama Koridor atau Nama Rute yang mencakup awal dan akhir untuk setiap rute.
9. `direction:` 0 untuk pergi, 1 untuk kembali. Menunjukkan arah rute.
10. `tapInStops:` ID pemberhentian masuk (tap in) untuk mengidentifikasi nama pemberhentian.
11. `tapInStopsName:` Nama pemberhentian masuk di mana pelanggan melakukan tap in.
12. `tapInStopsLat:` Lintang dari pemberhentian masuk.
13. `tapInStopsLon:` Bujur dari pemberhentian masuk.
14. `stopStartSeq:` Urutan pemberhentian, misalnya pemberhentian pertama, kedua, dan seterusnya. Berkaitan dengan arah.
15. `tapInTime:` Waktu tap in. Tanggal dan waktu.
16. `tapOutStops:` ID pemberhentian keluar (tap out) untuk mengidentifikasi nama pemberhentian.
17. `tapOutStopsName:` Nama pemberhentian keluar di mana pelanggan melakukan tap out.
18. `tapOutStopsLat:` Lintang dari pemberhentian keluar.
19. `tapOutStopsLon:` Bujur dari pemberhentian keluar.
20. `stopEndSeq:` Urutan pemberhentian, misalnya pemberhentian pertama, kedua, dan seterusnya. Berkaitan dengan arah.
21. `tapOutTime:` Waktu tap out. Tanggal dan waktu.
22. `payAmount:` Jumlah yang dibayar oleh pelanggan. Beberapa gratis, beberapa tidak.

**2. Apakah ada rute yang secara konsisten mengalami kepadatan penumpang?**
- Justifikasi: Mengidentifikasi rute yang padat akan membantu dalam alokasi sumber daya dan armada yang lebih baik.
- Kolom Relevan: id transaksi, nama koridor, halte masuk, halte keluar.
- Bantuan Analis Data: Menghitung jumlah transaksi per rute untuk menentukan kepadatan.

**Analisis dari pertanyaan-pertanyaan ini akan membantu Divisi Manajemen Operasional Transjakarta dalam membuat keputusan yang lebih informatif dan strategis untuk meningkatkan efisiensi operasional.**
