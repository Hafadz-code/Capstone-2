# Capstone-2
## Latar Belakang
Capstone Modul 2 (New York City TLC Trip Record)
berdasarkan situs resmi TLC berbunyi:
"*The New York City Taxi and Limousine Commission (TLC), created in 1971, is the agency responsible for licensing and regulating New York City's Medallion (Yellow) taxi cabs, for-hire vehicles (community-based liveries, black cars and luxury limousines), commuter vans, and paratransit vehicles. The Commission's Board consists of nine members, eight of whom are unsalaried Commissioners. The salaried Chair/ Commissioner presides over regularly scheduled public commission meetings and is the head of the agency, which maintains a staff of approximately 600 TLC employees*.

*Over 200,000 TLC licensees complete approximately 1,000,000 trips each day. To operate for hire, drivers must first undergo a background check, have a safe driving record, and complete 24 hours of driver training. TLC-licensed vehicles are inspected for safety and emissions at TLC's Woodside Inspection Facility*"

Sumber dapat diakses pada link berikut [klik link](https://www.nyc.gov/site/tlc/about/about-tlc.page).

berdasarkan data yang diterima terdapat penugasan dalam melakukan analisis yang dapat memberikan insight bagi perusahaan agar dapat memberikan dampak positif bagi perusahaan dari hasil analisis dan rekomendasi yang disarankan

## Pernyataan Masalah
kapan waktu yang tepat untuk menyediakan sejumlah layanan transportasi tambahan untuk memberikan pelayanan yang optimal dan mendapatkan revenue yang maksimal?

varibel yang digunakan dalam data analisis untuk menjawab problem statement diatas adalah: lpep_pickup_datetime berdasarkan Hari dan Jam PULocationID untuk melihat jumlah trip dan lokasi order total_amount untuk melihat jumlah pendapatan

# Goals
1. potensi peningkatan kepuasan pelayanan pelanggan melalui peningkatan jumlah layanan yang disediakan
2. potensi estimasi peningkatan pendapatan

# Batasan masalah
1. tidak mengukur dan memperhitungkan nilai/indeks tingkat kepuasan pelanggan.
2. tidak menggunakan, membandingkan dan menguji metode-metode yang paling baik yang seharusnya digunakan.
3. rentang waktu dan lokasi yang digunakan sesuai dalam database
4. penggunaan analisis adalah karena pada setiap lokasi pasti ada drivernya yang standby, jika mau di tingkatkan pelayanannya maka harus menambah sarananya dan tidak ada alternatif lain (terutama pada lokasi yang berpotensi tidak membutuhkan banyaknya layanan berdasarkan rendahnya permintaan di daerah tersebut) naka analisis dilakukan dari waktu, sebab tidak setiap waktu ada drivernya dan jika ingin meningkatkan pelayanan maka dapat menambah layanan pada waktu tertentu atau dengan alternatif pemindahan sarana pada lokasi yang sepi ke lokasi yang padat pada titik puncak waktunya dan kembali pada posisi semula pada saat kembali normal.

# Perhitungan dan Pengujian statistik
1. perhitungan asumsi jumlah sarana (driver/armada) berdasarkan jumlah trip
2. penggunaan statistik deskriptif untuk menggambarkan sebaran trip pada waktu tertentu
3. prediksi rata-rata kenaikan jumlah trip dengan penambahan jumlah sarana (driver/armada)
5. menguji kausal penyebab 1 ke penyebab sebelumnya
4. menguji korelasi permasalahan terhadap akar penyebab
4. menguji korelasi peningkatan sarana (driver/armada) terhadap peningkatan pendapatan secara total
3. menguji korelasi keuntungan saat ini dibanding keuntungan sesudah rekomendasi
1. menghitung potensi pendapatan total setelah menindak-lanjuti rekomendasi

2. berdasarkan penentuan SCR atau situation, complication dan resolution maka dapat didefinisikan bahwa dari hasil data analisis didapatkan


##  situation:
informasi yang didapat dari hasil analisis:
1. Jumlah total trip: 678181.
2. Rata-rata trip dalam 1 hari: 9929
1. Rata-rata lama trip: 0.3006727851668353 jam
2. total jumlah (sarana/driver) : 426 (sarana/driver)
3. Rata-rata jumlah orderan untuk 1 (sarana/driver) per hari: 23 orderan
4. Rata-rata total pendapatan disetiap hari (tgl 1-31): $ 22.57
5. Rata-rata total pendapatan disetiap jam (tgl 1-31): $ 0.94
6. Median trip harian: 9929.0
7. Titik Puncak harian: 11190
8. hari titik puncak: Tuesday
9. Median trip dalam jam: 3207.0
10. Titik Puncak pada jam: 5216
11. jam titik puncak: 18.00
12. Persentase kenaikan titik puncak harian: 12.70 %
13. Persentase kenaikan titik puncak harian: 39.32 %
14. jumlah trip pada titik terendah harian: 8305
15. hari titik terendah: Sunday
16. jumlah trip pada titik terendah pada jam: 426
17. jam titik terendah: 05.00
18. 10 lokasi taxi-zone dengan order tertinggi pada titik puncak harian: 74, 75, 41, 166, 95, 82, 43, 97, 7 dan 244
19. 10 lokasi taxi-zone dengan order tertinggi pada titik puncak jam:
74, 75, 41, 166, 95, 82, 43, 97, 7 dan 244
20. 10 lokasi taxi-zone dengan order terendah pada titik puncak jam: 241,120, 220, 18, 35, 70, 203, 93, 213,26
21. 10 lokasi taxi-zone dengan order terendah pada titik puncak harian: 194, 68, 161, 100, 143, 170, 88, 221, 79, 58


## complication:
terdapat alasan dibalik permasalahan yang dapat dianalisis bahwa
1. terdapat sebaran trip yang tidak merata pada hari tertentu dalam 1 minggu dan pada jam tertentu dalam 1 hari
2. terdapat sebaran trip yang tidak merata pada lokasi penjemputan/pelayanan
3. terdapat jumlah trip rata-rata yang dapat mengasumsikan jumlah sarana yang ada dalam 1 hari yang masih dapat dioptimalkan
4. terdapat jumlah rata-rata tarif regular untuk pendapatan atau harga satuan (tarif/trip) yang masih dapat dioptimalkan dengan kondisi khusus

tujuan pemecahan masalah diatas adalah:
mendapatkan potensi peningkatan kepuasan pelayanan pelanggan melalui peningkatan jumlah layanan yang disediakan sekaligus memberikan potensi estimasi peningkatan pendapatan melalui pengaturan penyebaran layanan

selanjutnya, perlu untuk mengembangkan analisis penyebab dan/atau dampak hingga didapatkan solusi yang efektif, efisien dan tepat sasaran

## Analisis Rekomendasi
solusi yang ingin didapatkan selayaknya dapat menyelesaikan masalah bahkan sekaligus memberikan dampak positif bagi perusahaan. metode yang ingin digunakan adalah dengan mendefinisikan terlebih dahulu permasalahannya dan memecahnya dalam bentuk akar penyebab sehingga dapat memberikan solusi pada akar penyebab tersebut bahkan membawa dampak positif.

Problem: Belum optimalnya pelayanan dan total pendapatan

akar penyebab:
keterbatasan layanan (sana/driver) pada suatu jam dan/atau hari tertentu yang berpotensi tidak dapat mengakomodir permintaan pada jam atau hari sibuk (titik puncak)
tidak meratanya sebaran waktu dan lokasi layanan (sarana/driver)
Resolution: terdapat 2 rekomendasi yang dapat diambil oleh perusahaan yaitu: rekomendasi:

menambah jumlah aset atau layanan (sarana/driver) pada waktu dan lokasi tertentu
menaikan harga tarif dasar pada waktu dan lokasi tertentu
Tindak lanjut dari 2 rekomendasi ini sulit untuk dilakukan karena:

menambah jumlah aset akan menambah anggaran investasi sehingga membutuhkan dana yang tidak sedikit, selain itu pada saat hari dan jam normal maka aset berpotensi akan menganggur (idle)
menaikan harga tarif dasar pada waktu tertentu akan berpotensi menurunkan kepuasan pelanggan pada rentang waktu tersebut diluar dari titik puncaknya
sehingga perlu adanya rekomendasi alternatif yaitu:

memindahkan sementara sebaran aset pelayanan (sarana/driver) pada waktu dan lokasi pada saat titik puncak.
memberikan harga tambahan hanya pada saat titik puncak terjadi.

## Resolution:
memindahkan sementara sebaran aset pelayanan (sarana/driver) pada waktu dan lokasi pada saat titik puncak
memberikan harga tambahan hanya pada saat titik puncak terjadi

Menghitung dampak positif penerapan rekomendasi 1
setting pemindahan sarana berdasarkan titik puncak harian:
10 sarana dari lokasi taxi-zone (order terendah pada titik puncak) harian, yaitu :194, 68, 161, 100, 143, 170, 88, 221, 79 dan 58
menuju 10 lokasi taxi-zone dengan order tertinggi pada titik puncak harian yaitu: 74, 75, 41, 166, 95, 82, 43, 97, 7 dan 244

setting pemindahan sarana berdasarkan jam titik puncak:
10 sarana dari lokasi taxi-zone (order terendah pada titik puncak) jam, yaitu :241, 120, 220, 18, 35, 70, 203, 93, 213 dan 26
menuju 10 lokasi taxi-zone dengan order tertinggi pada titik puncak jam, yaitu: 74, 75, 41, 166, 95, 82, 43, 97, 7 dan 244

estimasi pendapatan jika memindahkan sarana berdasarkan hari puncak: $ 84086.42048362295 / minggu
estimasi pendapatan jika memindahkan sarana berdasarkan jam puncak: $ 3503.60085348429 / hari

Menghitung dampak positif penerapan rekomendasi 2
penambahan $1 per orderan untuk setiap hari titik puncak harian (Tuesday) dapat memberikan perbedaan terhadap pendapatan
pendapatan tambahan jika terdapat penyusuaian tarif titik puncak harian: $ 14914.979629860885 minggu

Total pemasukan jika diterapkan Rekomendasi 1 dan 2
Total estimasi pendapatan jika menerapkan 2 rekomendasi yang disarankan adalah: $ 504617.2269119483 per bulan januari
