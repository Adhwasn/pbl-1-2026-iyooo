1. Profil Organisasi / Unit Usaha
    Nama unit usaha: Frenza Mart
    Jenis usaha / layanan: Toko kelontong yang menyediakan berbagai macam barang dan kebutuhan pokok sehari-hari seperti semobako, makanan ringan, minuman dan perlengkapan lain rumah tangga untuk masyarakat 
    Lokasi: Jl. Singoranu, Giwangan, Kec. Umbulharjo, Kota Yogyakarta, DIY 55163 (±1.0 km dari Kampus UAD 4)
    Deskripsi singkat operasional: Frenza Mart melayani masyarakat umum dan mahasiswa sekitar dalam pemenuhan kebutuhan harian. Operasional dimulai dari pagi hingga malam hari, di mana proses pelayanan pembeli, pengecekan harga barang, pencatatan transaksi kasir, dan rekapitulasi omzet harian masih dikelola secara konvensional (manual menggunakan buku catatan dan kalkulator).

2. Deskripsi Masalah Utama

    Masalah utama: 
    1. Pencatatan transaksi dan inventaris yang masih dilakukan secara manual menggunakan kalkulator dan catatan buku di Frenza Mart (kondisi As-Is) menyebabkan bottleneck operasional berupa waktu transaksi kasir yang lambat (30 – 60 detik/pelanggan) karena penjaga harus mengingat atau mengecek harga secara manual, keterlambatan pemantauan stok akibat selisih pencatatan 1 - 2 kali per minggu pada beban puncak 5–15 orang/jam, serta waktu rekapitulasi harian pemilik usaha yang memakan waktu hingga 10 – 25 menit setiap malam
    2.  Pihak yang terdampak : Penjaga toko (mengalami kerepotan saat antrean pembeli memuncak karena harus menghitung manual) staff danpemilik usaha (menghabiskan waktu ekstra di malam hari untuk mencocokkan omzet serta menghadapi risiko selisih stok barang).
    3.  Keparahan : Terjadi setiap hari pada jam-jam sibuk operasional toko dan setiap malam saat penutupan toko


3. Batasan Sistem (Scope)

    Diselesaikan dalam proyek ini: 
    1.  Pencatatan transaksi kasir toko berbasis konsol C++ (CLI).
    2.  Manajemen inventaris / pemantauan stok barang dagangan.
    3.  Pencetakan ringkasan rekapitulasi pendapatan harian untuk pemilik.

Tidak diselesaikan (dan alasan): 
    1.  Sistem manajemen keuangan lanjutan (laba rugi & pajak) — Terlalu kompleks untuk batasan PBL Level 1 yang berfokus pada pencatatan transaksi operasional dasar.
    2.  Pengelolaan database supplier & pemesanan otomatis serta Pengadaan barang ke supplier eksternal dilakukan secara berkala secara langsung, di luar ruang lingkup sistem kasir lokal.
    3.  Pengelolaan multi-cabang atau sistem berbasis cloud — Mitra Frenza Mart saat ini beroperasi terpusat secara mandiri di satu lokasi.
    Asumsi yang dipakai:   
    Perangkat komputer/laptop dengan compiler C++ tersedia di area operasional atau digunakan oleh tim pengembang untuk mendemonstrasikan prototipe kepada mitra

4. Data Kuantitatif Pendukung
Indikator 	Nilai/Baseline 	Sumber Data 	Tanggal
Waktu layanan transaksi kasir 	30 – 60 detik / pelanggan 	Observasi lapangan 	26/10
Durasi rekapitulasi harian 	10 – 25 menit / malam 	Wawancara pemilik 	26/10
Frekuensi selisih stok 1 - 2 kali / minggu Wawancara pengelola	 26/10		
5. Pernyataan Kebutuhan Awal (ringkasan ke D2)

    Kebutuhan inti 1: Kemampuan memasukkan daftar belanjaan dan menghitung total harga secara otomatis tanpa kalkulator manual.
    Kebutuhan inti 2: Pembaruan (update) jumlah sisa stok barang di sistem secara otomatis setiap kali terjadi transaksi penjualan.
    Kebutuhan inti 3: Penyediaan laporan ringkasan rekapitulasi pendapatan harian yang akurat dan cepat di akhir sesi operasional.
    Kebutuhan inti 4: Antarmuka berbasis konsol teks (C++) yang sederhana, intuitif, dan mudah dioperasikan oleh penjaga toko.


6. Daftar Rujukan / Bukti

    Observasi lapangan tanggal 27 October 2026
    Wawancara pemilik tanggal 27 Octberber 2026

Status: ⬜ Draf → ⬜ Review Tim → ⬜ Validasi Pemilik → ⬜ Final (Gate 1)