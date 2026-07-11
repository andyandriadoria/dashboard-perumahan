# Perubahan Dashboard SIRUMAH v36

## Penataan fungsi tombol

- Toolbar utama hanya memuat filter **Kecamatan** dan **Mode Internal/Publik**, karena keduanya berlaku untuk seluruh dashboard.
- Tombol **Muat Ulang Data GitHub** dan **Pilih Excel Lokal** dipindahkan ke menu **Integrasi SIRUMAH**.
- Tombol **Cetak/PDF** dan **Export CSV** ditempatkan pada menu yang relevan:
  - Beranda: Cetak/PDF.
  - Data Perumahan: Cetak/PDF dan Export CSV.
  - Peta Perumahan: Cetak/PDF dan Export CSV data lokasi.
  - Backlog & MBR: Cetak/PDF dan Export CSV.
  - RTLH & RLH: Cetak/PDF dan Export CSV.
  - PSU & RTH: Cetak/PDF dan Export CSV rekap/ranking.
  - RUSUNAWA: Cetak/PDF dan Export CSV.
  - Layanan & Pengaduan: Cetak/PDF dan Export CSV.
  - Kolaborasi: Cetak/PDF dan Export CSV.
  - Laporan: Cetak/PDF.

## Sumber data

- Tombol **Data Bawaan** dihapus.
- Seluruh data contoh yang tertanam di HTML dihapus.
- Nilai awal seluruh indikator, tabel, backlog, RTLH/RLH, RUSUNAWA, layanan, dan kolaborasi adalah **0/kosong**.
- Dashboard hanya terisi setelah workbook Excel resmi berhasil dimuat dari:

  `data/Template_Resmi_Database_SIRUMAH.xlsx`

  atau setelah pengguna memilih Excel lokal pada menu Integrasi.
- Jika pemuatan Excel gagal, dashboard tetap bernilai 0 dan menampilkan pesan kegagalan tanpa memakai data contoh.

## Cetak dan ekspor

- Cetak/PDF hanya mencetak menu yang sedang dipilih, bukan seluruh dashboard.
- Cetak Data Perumahan menampilkan seluruh hasil filter, bukan hanya halaman tabel yang sedang terlihat.
- Export CSV Data Perumahan mengekspor seluruh hasil filter.
- Dalam Mode Publik, kolom Direktur/Pelaksana tidak ikut masuk ke CSV Data Perumahan.
- Export CSV pada menu lain mengambil tabel yang sedang tampil dan mengikuti filter aktif.
