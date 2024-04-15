# Capstone Project Module-2 TransJakarta (Public Transportation Transaction)

# **Latar Belakang dan Identifikasi Masalah**  
  
TransJakarta adalah sebuah sistem transportasi Bus Rapid Transit (BRT) pertama di Asia Tenggara dan Selatan yang beroperasi sejak tahun 2004 di Jakarta, Indonesia. TransJakarta dirancang sebagai moda transportasi massal pendukung aktivitas ibukota yang sangat padat. Dengan jalur lintasan terpanjang di dunia (251.2 km), serta memiliki 287 halte yang tersebar dalam 13 koridor.

TransJakarta yang awalnya beroperasi mulai jam 05.00 –  22.00 WIB, kini beroperasi 24 jam. Hal tersebut berkenaan dengan semakin tingginya minat masyarakat untuk menggunakan moda transportasi TransJakarta. Data Badan Pusat Statistik (BPS) menyebutkan sepanjang Januari 2024, jumlah penumpang Transjakarta mencapai 30.934.491 orang. Angka ini meningkat 6,83% dibandingkan Desember 2023 dan mengalami peningkatan 4,66% dibandingkan Januari 2023 (Jakarta.bps.go.id).

Minat masyarakat untuk menggunakan transportasi TransJakarta dikarenakan tarif yang relatif murah jika dibandingkan dengan beberapa pilihan moda transportasi lainnya seperti MRT, LRT serta moda transportasi berbasis online. Namun, sejak beroperasional pada tahun 2004, banyak kekurangan dalam sistem pelayanan TransJakarta, seperti kurangnya armada untuk menampung penumpang yang menyebabkan over capacity serta masih terdapat koridor yang belum steril dari kendaraan pribadi yang menyebakan waktu perjalanan tidak optimal.

# **Tujuan Analisa Data**  
1. Mengetahui waktu terpadat (peak hour) pada moda transportasi TransJakarta
2. Mengetahui lokasi terpadat asal dan tujuan berdasarkan data Tap-In dan Tap-Out pengguna TransJakarta
3. Mengetahui koridor terpadat dari pengguna TransJakarta
4. Merekomendasikan beberapa saran yang dapat menjadi pertimbangan oleh TransJakarta dalam meningkatkan kualitas layanan berdasarkan data transaksi pengguna serta penambahan armada TransJakarta

# **Dataset**

Dataset bersumber dari kaggle dan dapat diunduh pada Link : https://www.kaggle.com/datasets/dikisahkan/transjakarta-transportation-transaction?select=dfTransjakarta.csv.  
|No. | Nama Kolom | Keterangan |
|----|------------|------------|
|1.	|transID| Unique transaction id for every transaction|
|2.	|payCardID| Customers main identifier. The card customers use as a ticket for entrance and exit.|
|3.	|payCardBank| Customers card bank issuer name|
|4.	|payCardName| Customers name that is embedded in the card.|
|5.	|payCardSex| Customers sex that is embedded in the card|
|6.	|payCardBirthDate| Customers birth year|
|7.	|corridorID| Corridor ID / Route ID as key for route grouping.|
|8.	|corridorName| Corridor Name / Route Name contains Start and Finish for each route.|
|9.	|direction| 0 for Go, 1 for Back. Direction of the route.|
|10.|tapInStops| Tap In (entrance) Stops ID for identifying stops name|
|11.|tapInStopsName| Tap In (entrance) Stops Name where customers tap in.|
|12.|tapInStopsLat| Latitude of Tap In Stops|
|13.|tapInStopsLon| Longitude of Tap In Stops|
|14.|stopStartSeq| Sequence of the stops, 1st stop, 2nd stops etc. Related to direction.|
|15.|tapInTime| Time of tap in. Date and time|
|16.|tapOutStops| Tap Out (Exit) Stops ID for identifying stops name|
|17.|tapOutStopsName| Tap out (exit) Stops Name where customers tap out.|
|18.|tapOutStopsLat| Latitude of Tap Out Stops|
|19.|tapOutStopsLon| Longitude of Tap Out Stops|
|20.|stopEndSeq| Sequence of the stops, 1st stop, 2nd stops etc. Related to direction.|
|21.|tapOutTime| Time of tap out. Date and time|
|22.|payAmount| The number of what customers pay. Some are free. Some not.|

# **Data Preparation**

1. Mengecek Data Duplikat
2. Menghitung Missing  Values
3. Menghitung Persentase Missing Values

# **Data Cleaning**

# **Analisa Data**
1. Analisa Statistika Deskriptif
2. Analisa Statistika Deskriptif untuk Data Kategorikal
   - Menganalisa Peak Hour TransJakarta
   - Menganalisa jumlah tapIn dan tapOut pada setiap halte TransJakarta
   - Menganalisa usia pengguna TransJakarta
   - Menganalisa corridor mana yang memiliki penumpang terbanyak & terdikit
   
# **Kesimpulan Dan Saran**

**Kesimpulan**  
Berdasarkan hasil Analisa Data, dapat disimpulkan bahwa:
* Waktu Peak Hour TransJakarta adalah pada pagi hari pukul 06.00 WIB dan sore hari pukul 17.00 WIB 
* TapIn terbanyak ada pada halte BKN sebanyak 274 taps dan tapOut terbanyak ada pada halte Penjaringan sebanyak 208 taps
* Usia terbanyak pada penggunaan TransJakarta adalah pada tahun kelahiran 1992,1994,1981,1987,1985 (32 Tahun, 30 Tahun, 43 Tahun, 37 Tahun, 39 Tahun)
* Pengguna TransJakarta paling banyak adalah pada koridor Cibubur - Balai Kota sebanyak 362 pengguna. Sedangkan, pengguna TransJakarta paling sedikit adalah pada koridor Kampung Rambutan - Blok M sebanyak 16 pengguna.

**Saran**

* Menambah jumlah perjalanan TransJakarta di jam sibuk untuk menambah income dan juga membuat pengguna tidak terlalu menumpuk agar pengguna merasa nyaman.
* Mengurangi jumlah perjalanan TransJakarta pada waktu siang hari (Pukul 12.00-15.00 WIB) dikarenakan pengguna pada waktu tersebut dapat dilihat sangat sedikit.
* Menambah armada pada daerah BKN dan Penjaringan karena tapIn dan tapOut terbanyak ada pada daerah tersebut.
* Mengurangi armada TransJakarta untuk koridor Kampung Rambutan - Blok M karena memiliki pengguna yang sedikit, pengalokasian TransJakarta bisa untuk Koridor Cibubur - Balai Kota karena memiliki pengguna terbanyak rata rata setiap harinya.

**Tableau**
https://public.tableau.com/views/CapstoneProjectModul2-JCDSPurwadhika/Story1?:language=en-US&publish=yes&:sid=&:display_count=n&:origin=viz_share_link





