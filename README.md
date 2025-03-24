# Tugas Organisasi dan Struktur Data

nama: Indah Damaiyanti
Nim: 09011182429030
Kelas: SKU2B

1. Struktur Antar Hubungan dan Contohnya
Struktur antar hubungan (interconnection structure) dalam sistem komputer merujuk pada mekanisme yang menghubungkan berbagai komponen komputer, seperti CPU, memori, dan perangkat I/O. Struktur ini memungkinkan terjadinya transfer data dan sinyal kontrol antar komponen.
Berikut adalah beberapa struktur antar hubungan utama:
 * Bus:
   * Bus adalah jalur komunikasi bersama yang menghubungkan beberapa perangkat.
   * Contoh: Sistem bus pada motherboard yang menghubungkan CPU, memori, dan slot ekspansi.
 * Hierarki Bus:
   * Struktur ini menggunakan beberapa bus dengan tingkat kecepatan dan prioritas yang berbeda.
   * Contoh: Bus lokal untuk CPU dan memori, bus sistem untuk perangkat berkecepatan tinggi, dan bus ekspansi untuk perangkat I/O.
 * Switching:
   * Struktur ini menggunakan switch untuk menghubungkan perangkat secara dinamis.
   * Contoh: Jaringan Ethernet yang menggunakan switch untuk menghubungkan komputer dan perangkat jaringan lainnya.
 * Point-to-Point Interconnect:
   * Struktur ini menghubungkan dua perangkat secara langsung.
   * Contoh: Sambungan antara CPU dan memori utama.
2. Penyebab Penurunan Kinerja pada Bus dengan Banyak Modul/Perangkat
Ketika terlalu banyak modul atau perangkat terhubung ke bus, kinerja sistem dapat menurun karena beberapa faktor:
 * Kontensi Bus:
   * Semakin banyak perangkat yang menggunakan bus, semakin besar kemungkinan terjadinya konflik akses.
   * Hal ini menyebabkan perangkat harus menunggu giliran untuk menggunakan bus, yang meningkatkan waktu tunggu dan menurunkan throughput.
 * Kapasitas Bus Terbatas:
   * Setiap bus memiliki kapasitas transfer data maksimum.
   * Jika jumlah data yang ditransfer melebihi kapasitas ini, bus akan mengalami kemacetan, yang menyebabkan penundaan dan penurunan kinerja.
 * Propagasi Sinyal:
   * Semakin panjang jalur bus dan semakin banyak perangkat yang terhubung, semakin besar kemungkinan terjadinya distorsi sinyal.
   * Hal ini dapat menyebabkan kesalahan data dan memerlukan transmisi ulang, yang menurunkan kinerja.
3. Prioritas Perangkat dan Waktu Tunggu
 * Dalam sistem bus dengan prioritas, perangkat dengan prioritas rendah biasanya memiliki waktu tunggu rata-rata yang lebih singkat karena mereka diizinkan untuk menggunakan bus hanya ketika perangkat dengan prioritas lebih tinggi tidak membutuhkannya.
 * Alasan perangkat berprioritas 16 memiliki waktu tunggu rata-rata paling rendah:
   * Biasanya pada sistem bus, perangkat yang memiliki prioritas lebih rendah, contohnya prioritas 16, akan memiliki kesempatan menggunakan bus ketika perangkat-perangkat yang memiliki prioritas lebih tinggi sedang tidak menggunakan bus. Sehingga waktu tunggu rata-rata yang didapatkan oleh perangkat prioritas 16 menjadi lebih rendah.
 * Kondisi di mana hal ini tidak berlaku:
   * Jika perangkat dengan prioritas tinggi terus-menerus menggunakan bus, perangkat dengan prioritas rendah mungkin mengalami waktu tunggu yang sangat lama.
   * Jika terjadi kesalahan dalam mekanisme prioritas, perangkat dengan prioritas rendah mungkin tidak mendapatkan akses ke bus sama sekali.
