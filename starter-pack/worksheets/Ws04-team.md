WS04: Problem Identification & Scope
Mata Kuliah: Konsep Sistem Informasi (KSI)
Kerangka Kerja: Project-Based Learning (PBL) Level 1
Fase Learning Spine: Fase 2 — Frame (Problem Discovery & Scope)
Minggu / Alokasi Waktu: Minggu 2 / 14 Jam Belajar
Sub-CPMK / SFIA: S-01.1 (Introduce - Problem Framing) | SFIA BUSA L1 (Business Analysis), IRMG L1
Penanggung Jawab Fase: Phase Lead 2 (Frame — Mahasiswa B)
Keterkaitan Deliverable: Sumber Utama Penyusunan Deliverable D1 (Problem Brief - TPL-01)

________________________________________
1. Identifikasi Tim & Objek Proyek
Elemen Informasi	Rincian Identitas Kelompok & Mitra
Nama Kelompok / Kelas	    :   Iyooo / A
Phase Lead 2 (Frame - M2)	:   Adhwa Shauqi Nabil - 2600016003
Nama UMKM Mitra Lapangan	:   Frenzy mart (toko kelontong)
Pemilik / Kontak Mitra	    :   Mba 

________________________________________
2. Matriks Problem Framing & Analisis Akar Masalah (Root Cause Analysis)
Gunakan temuan kuantitatif dari WS03 untuk memisahkan antara Gejala Permukaan (Symptoms) dan Akar Masalah Utama (Root Cause) operasional bisnis mitra:

No	Kategori Observasi	Gejala Permukaan (Symptoms)	Akar Masalah Operasional (Root Cause)	Bukti Kuantitatif (Baseline Data)
1	Proses Transaksi Kasi      : Antrean pembeli saat
jam sibuk dan proses hitung manual. Penjaga toko harus mengingat/mengecek harga manual dan
menghitung total belanja memakai kalkulator. Rata-rata waktu transaksi = 60 - 80 detik/pelanggan.
2	Pengelolaan Stok Barang    : Risiko kekurangan stok barang di rak atau selisih pencatatan inventaris. Pengurangan stok tidak tercatat otomatis saat transaksi; pemantauan stok masih secara visual di rak. Frekuensi selisih pencatatan = 1 - 2 kali/minggu.
3	Rekapitulasi Keuangan      : Staff kerepotan merekap pendapatan harian tiap malam.Penghitungan total penjualan harian masih mengandalkan catatan buku dan kalkulator manual. Durasi rekap harian = 15 – 30 menit/malam.
________________________________________
3. Perumusan Problem Statement Kontekstual
Berdasarkan analisis di atas, rumuskan Problem Statement utama dalam 1–2 paragraf terstruktur. Petunjuk: Hindari mendefinisikan masalah sebagai "Mitra belum memiliki aplikasi Python/komputer". Definisikan dari hambatan bisnis nyata mitra!

Rumusan Problem Statement Kelompok :
Pencatatan transaksi dan inventaris yang masih dilakukan secara manual menggunakan kalkulator
dan catatan buku di Frenza Mart (kondisi As-Is) menyebabkan bottleneck operasional berupa
waktu transaksi kasir yang lambat (60 - 80 detik/pelanggan) karena penjaga harus mengingat
harga dan menghitung manual, keterlambatan pemantauan stok akibat selisih pencatatan 1 - 2 kali per minggu pada beban puncak 5–15 orang/jam, serta waktu rekapitulasi harian pemilik usaha yang memakan waktu hingga 15 – 30 menit tiap malam. Kondisi ini menghambat efisiensi
operasional dan potensi pertumbuhan omzet mitra

________________________________________
4. Menetapkan Batasan Sistem (System Boundary / Scope Alignment)
Untuk mencegah terjadinya pembengkakan fitur (Scope Creep) yang membahayakan penyelesaian proyek dalam 1 semester, tentukan secara tegas apa yang Masuk Cakupan (In-Scope) dan apa yang Di Luar Cakupan (Out-of-Scope):

 ┌───────────────────────────────────────────┐
 │                    SYSTEM BOUNDARY (BATASAN SISTEM)                           │
 │                                                         	                     │
 │   [ IN-SCOPE: Fitur yang Akan Dibangun ]                                      │
 │   1. Pencatatan transaksi kasir toko berbasis C++ (CLI).                      │
 │   2. Stock barang daganan                                                     │
 │   3. Pencetakan ringkasan rekapitulasi pendapatan harian                      │
 │                                                                               │
 │───────────────────────────────────────────                                    │
 │                                                                               │
 │   [ OUT-OF-SCOPE: Di Luar Cakupan Proyek ]                                    │
 │   1. Sistem manajemen keuangan (laba rugi)                                    │
 │   2. engelolaan database supplier & pemesanan otomatis                        │
 │   3. Pengelolaan multi-cabang atau sistem berbasis cloud                                │   └────────────────────────────────────────────┘
Tabel Penegasan Cakupan Proyek (Scope Alignment Table)
No	Modul / Fitur Sistem	Status Cakupan (In-Scope / Out-of-Scope)	Alasan Pertimbangan Kelayakan (O'Brien)
1	Input Transaksi & Kalkulasi Total IN-SCOPE	Kelayakan Operasional: Sangat dibutuhkan penjaga toko untuk memepercepat transaksi dan menghindari kesalahan dalam menghitung
2	Update Stok Otomatis	IN-SCOPE	Kelayakan Teknis: Membantu pemantauan sisa stok di rak berbasis struktur data C++.
3	Laporan Rekap Harian (Laba/Rugi)	IN-SCOPE	Kelayakan Ekonomi: Memberikan nilai  Value of Information bagi pemilik untuk rekap malam.
4	Pembayaran Online / Payment Gateway	OUT-OF-SCOPE	Terlalu kompleks untuk batasan PBL Level 1 yang berfokus pada pencatatan transaksi operasional dasar.
5	Multi-Branch / Banyak Cabang	OUT-OF-SCOPE	Pengadaan barang ke supplier eksternal dilakukan secara berkala secara langsung, di luar ruang lingkup sistem kasir lokal.

________________________________________
5. Target Metrik Keberhasilan Solusi (To-Be Targets)
Tentukan target kuantitatif perbaikan yang ingin dicapai melalui solusi sistem informasi To-Be:

Indikator Kinerja	Kondisi As-Is (Baseline)	Target To-Be (Expected)	Estimasi Persentase Peningkatan
Waktu Pelayanan Transaksi Kasir	30 – 60 detik / pelanggan	< 30 detik / pelanggan	Peningkatan efisiensi 44.4%
Durasi Rekapitulasi Harian	10 – 25 menit / malam	< 10 menit / malam	Penghematan waktu 71.4%
Akurasi Pencatatan Stok	Risiko selisih catatan nota	Akurasi > 98%	Penurunan tingkat kesalahan selisih stok

________________________________________
6. Refleksi & Lembar Pengesahan Phase Lead
A. Pertanyaan Refleksi Tim
1.	Bagaimana tim memastikan bahwa batasan proyek yang ditetapkan realistis untuk diselesaikan dalam 16 minggu?
●	Jawab: Dengan membatasi ruang lingkup pada prototipe konsol berbasis C++ yang berfokus langsung pada inti masalah pencatatan transaksi kasir dan rekapitulasi harian toko kelontong.
2.	Apakah pemilik usaha mitra telah menyetujui batasan sistem yang diusulkan oleh kelompok?
●	Jawab: Ya, ruang lingkup telah diselaraskan dengan kebutuhan praktis operasional Frenza Mart
B. Tanda Tangan Pengesahan Phase Lead 2
Disusun oleh Phase Lead 2 (Frame): [ Adhwa Shauqi Nabil — 2600016003]
Tanggal Penyusunan: [ 27 October 2026 ]

Tanda Tangan Phase Lead 2: Tertanda_Adhwa_Shauqi_Nabil

Diverifikasi oleh Dosen Pengampu / Coach:
Tanggal: [ 27l ] | Status Checkpoint: [ APPROVED ]
Catatan Dosen: __________________________________________________

