# **WORKBOOK: LEMBAR KERJA MAHASISWA WS05** 

## **Formulasi Kebutuhan Fungsional: User Story & Acceptance Criteria** 

Mata Kuliah: **Konsep Sistem Informasi (KSI)** Kerangka Kerja: **Project-Based Learning (PBL) Level 1** Fase Learning Spine: **Fase 3 — Define (Minggu 3)** Sub-CPMK / SFIA: **S-01.1 (Intermediate - Problem Framing) & S-03.1 (Intermediate - Pemetaan SI)** | **SFIA BUSA L1, REQM L2** Keterkaitan Deliverable: **Bahan Utama Deliverable D2 (System & Solution Design - TPL-02)** 

### **1. Identifikasi Kelompok & Rotasi Kepemimpinan** 

- **Nama Kelompok** : IYOOO 

- **Objek UMKM Mitra** : Frenza Mart 

- **Phase Lead 3 (Define)** : Adhwa Shauqi Nabil 

- **Anggota Tim** : 

   1. Nabila Luthfia Putri 

   2. Adhwa Shauqi Nabil 

   3. Taufiq Khairan Nafi 

### **2. Landasan Konseptual: Analisis Sistem "What" vs "How"** 

Dalam tahap _Systems Analysis_ , fokus utama tim adalah menentukan **APA (** **_What_ )** yang dibutuhkan pengguna bisnis untuk memecahkan masalahnya, **BUKAN BAGAIMANA (** **_How_ )** sistem dibangun secara teknis (Marakas & O'Brien, 2013). 

- **User Story** merepresentasikan kebutuhan fungsional dari sudut pandang pengguna bisnis dengan pola: 

$$\text{"Sebagai Pemilik usaha, Saya Melihat ringkasan total pendapatan harian serta rekap jumlah transaksi saat penutupan toko, Sehingga proses rekapitulasi harian menjadi akurat"}$$ 

- **Acceptance Criteria (Given-When-Then)** mendefinisikan batas kondisi kapan sebuah fitur dinyatakan selesai dan memenuhi syarat penerimaan pengguna (Rainer et al., 2021). 

### **3. Workspace A: Formulasi User Story Fungsional** 

Petakan minimal **3 User Story Utama** yang langsung menjawab akar masalah pada D1 / WS04: 

#### **User Story 1 (Prioritas Utama / Core Feature)** 

- **Sebagai (** **_As a_ )** : 

Mba Dila : Penjaga toko 

- **Saya ingin (** **_I want to_ )** : 

Memasukan nama barang dan jumlah beli supaya system menghitung total harga secara otomatis 

- **Sehingga (** **_So that_ )** : 

Waktu pelayanan transaksi menjadi lebih cepat dan menghindari kesalahan dari perhitungan manual 

#### **User Story 2 (Fitur Manajemen Stok / Data)** 

- **Sebagai (** **_As a_ )** : 

Bu Frenza : Pemilik Usaha 

- **Saya ingin (** **_I want to_ )** : 

Melihat jumlah stok barang serta memastikan stok berkurang tiap pembelian transaksi 

- **Sehingga (** **_So that_ )** : 

Pemilik toko dapat memantau ketersediaan barang dari manapun saja tanpa harus mengecehk rak satu persatu 

#### **User Story 3 (Fitur Pelaporan / Informasi)** 

- **Sebagai (** **_As a_ )** : 

Bu Frenza : Pemilik Usaha 

- **Saya ingin (** **_I want to_ )** : 

   - Dapat memantau total omset harian dan rekap jumlah transaksi saat penutupan 

- **Sehingga (** **_So that_ )** : 

proses rekapitlasi harian menjadi akurat 

### **4. Workspace B: Acceptance Criteria Berbasis Skenario (Given-WhenThen)** 

Susun kriteria penerimaan terstruktur untuk **User Story 1** (mencakup Skenario Sukses dan Skenario Penanganan Eror): 

#### **Skenario 1A: Transaksi Penjualan Berhasil (Happy Path)** 

- **Diberikan (** **_Given_ )** : 

Kasir berada di menu utama pencatan transaksi dan stok produk tercatat tersedia 

- **Ketika (** **_When_ )** : 

Kasir memasukan nama produk, jumlah pembelian, dan menerima pembayaran tunai secara pas dari pembelia 

- **Maka (** **_Then_ )** : 

Sistem menghitung total belanja secara otomatis, menampilkan rincian transaksi sukses dengan uang kembalian Rp 0, serta langsung mengurangi jumlah sisa stok produk 

#### **Skenario 1B: Penanganan Pembayaran Kurang / Eror (Exception Path)** 

- **Diberikan (** **_Given_ )** : 

Total belanja transaksi di sistem menunjukkan nominal tertentu 

- **Ketika (** **_When_ )** : 

Kasir memasukkan nominal pembayaran uang tunai yang nilainya kurang dari total tagihan belanja. 

- **Maka (** **_Then_ )** : 

Sistem menolak pemrosesan transaksi, menampilkan pemberitahuan bahwa nominal pembayaran kurang, dan stok barang di sistem tidak berubah 

### **5. Workspace C: Catatan Validasi Kebutuhan dengan Mitra (Field Confirmation)** 

- **Tanggal Validasi** : 27/October/2026 

- **Narahubung Mitra** : Mba Dila (Staf Kasir) 

- **Hasil Konfirmasi User Story** : 

   - [V] Seluruh User Story disetujui mitra 

[X] Terdapat penyesuaian/revisi kebutuhan (Tuliskan revisi jika ada): 

### **6. Verifikasi Integritas AI (TPL-07) & Pengesahan** 

- **Penggunaan AI Co-pilot** : 

   - Apakah tim menggunakan AI untuk membantu merumuskan skenario _Given-WhenThen_ ? [ ] Ya  [V] Tidak 

_(Jika Ya, wajib melampirkan formulir_ **_TPL-07: AI Usage Disclosure & Verification Note_** _)_ . 

**Tanda Tangan Tim & Pengesahan Dosen** : 

● **Phase Lead 3** : _______________________ (Tanggal: __________) ● **Dosen Coach** : _______________________ (Tanggal: __________)  [ ] Approved 

