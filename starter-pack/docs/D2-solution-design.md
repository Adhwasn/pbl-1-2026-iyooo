# D2 — System & Solution Design

**Project**: Digital Problem Framing Mini Project — [Nama Unit Usaha]
**Tim**: [Nama anggota] | **Tanggal**: [DD/MM/YYYY] | **Versi**: [v1.0]
**Template**: TPL-02

> **Petunjuk**: Hapus teks dalam `[...]` setelah diisi.
> Worksheet terkait: WS05, WS06, WS07

---

## 1. Daftar Kebutuhan (User Story)

| # | User Story | Prioritas |
|---|---|---|
| 1 | | Sebagai Kasir toko, saya ingin memasukkan nama barang dan jumlah pembelian ke dalam sistem pencatatan transaksi sehingga total harga belanjaan dan uang kembalian dihitung secara otomatis oleh sistem | [Tinggi] |
| 2 | | Sebagai Pengelola Usaha, saya ingin memantau sisa stock barang secara langsung di system tiap kaliada transaksi penjualan yang berhasil | [Tinggi] |
| 3 | |Sebagai pengelola usaha, saya ingin melihat ringkasan total penpatan harian dan perhitungan penjualan secara praktis saat penutupan toko | [Sedang] |

## 2. Kriteria Penerimaan

| # | Kriteria Penerimaan (terukur & dapat diuji) |
|---|---|
| 1 |  | Sistem dapat menghitung total harga belanja dan uang kembalian dengan akurasi yang akurat dalam waktu <1 detik setelah proses input selesai |
| 2 | | Stock barang di system akan berkurang secara otomatis jika ada transaksi penjualan yang di nyatakan sukses |
| 3 | | Sistem akan menolak transaksi dan ada pemberitahuan jika nominal pembayaran kurang dari harga total penjualan, serta memastika stock data tidak berubah |
## 3. Success Metrics

| Metrik | Baseline (Sekarang) | Target | Cara Mengukur |
|---|---|---|---|
| Waktu rekapitulasi harian | 30-45 menit | [ <30 menit ] | Perbandingan durasi waktu saat penutupan sebelum dan sesudah menggunakan system |
| Keakuratan perhitungan transaksi |[ Sering terjadinya selisih saat menghitung manual] | 0% selisih (akurasi 100%) | Pencocokan total uang kas fisik di laci dengan rekapitulasi sistem. |

## 4. Desain Solusi

### 4.1 Konsep Solusi (ringkasan)

_[Satu paragraf bagaimana prototipe menjawab masalah dari D1]_

### 4.2 Peta Komponen (IPO)

```
Input  ──▶  Proses  ──▶  Output
  │                           │
  └───── Data/Penyimpanan ────┘
```

- **Input**: Nama ataupun code barang, jumlah pembelian barang dan nominal uang tunai pembayaran dari pembeli
- **Proses**: Memvalidasi ketersediaan stock, menghitung subtotal dan total belanja keseluruhan, menghitung uang kembalian, serta mwmperbarui sisa stock barang
- **Output**: Rincian struck transaksi di layar , status transaksi (sukses/gagal), nominal uang kembalian, serta laporan rekapitulasi pendapatan harian
- **Data/Penyimpanan**: Penyinpanan data master produk, daftar harga dan ketersidaan stock menggunakan struktur data berbasis memori dan file teks pendukung  

### 4.3 Flowchart & Pseudocode

_[Tempel flowchart di `assets/` dan tulis pseudocode di bawah]_

```
[PSEUDOCODE]
START
Tampilkan Menu Utama
Pilih Menu: 1. Transaksi Baru, 2. Cek Stok, 3. Rekap Harian, 4. Keluar
JIKA Pilih 1 (Transaksi Baru):
    ULANGI:
        Input Nama/Kode Barang & Jumlah Pembelian
        Cek Ketersediaan Stok
        JIKA Stok Mencukupi:
            Hitung Subtotal & Masukkan ke Keranjang Belanja
        JIKA TIDAK:
            Tampilkan Pesan "Stok Barang Tidak Cukup"
    SELESAI ULANGI
    Tampilkan Total Belanja Keseluruhan
    Input Nominal Pembayaran Uang Tunai dari Pembeli
    JIKA Pembayaran >= Total Belanja:
        Hitung Kembalian = Pembayaran - Total Belanja
        Kurangi Stok Barang di Sistem Secara Otomatis
        Simpan Data ke Rekapitulasi Pendapatan Harian
        Tampilkan Transaksi Berhasil & Rincian Kembalian
    JIKA TIDAK:
        Tampilkan Pesan Eror "Pembayaran Kurang" & Batalkan Pemotongan Stok
END

## 5. Hasil Validasi Pemilik Usaha

- **Tanggal validasi**: [27/10/2026]
- **Feedback staff**: Mbak dila selaku staff kasir masih memberikan masukan dan cacatan agar alur aplikasinya lebih disesuaikan dengan kebiasaan di toko. Yang dimana masukan ini sedang ditinjau oleh tim kami, dan belum dilaporkan secara final kepada Ibu Frenza selaku pengelola usaha 
- **Perubahan setelah validasi**: Tim kami akan menyesuaikan sedikit catatan alur operasionalnya agar mereka dapat mengetahui serta dapat digunakan oleh staff yang berada di toko sebelum nantinya dimintakan persetujuan oleh Ibu Frenza

---

**Status**: ⬜Draf → ⬜ Review Tim → ⬜ Validasi Pemilik → ⬜ Final (GATE 1)