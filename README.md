# Aplikasi Sistem Pendukung Keputusan Pemilihan Handphone Terbaik Menggunakan Metode SAW (Java NetBeans & MySQL)

Aplikasi ini merupakan sistem pendukung keputusan untuk pemilihan handphone terbaik menggunakan metode SAW, dibangun dengan **Java Swing** untuk antarmuka pengguna dan **MySQL** sebagai database.  
Aplikasi ini cocok digunakan untuk tugas akhir, studi kasus bisnis, atau pengambilan keputusan berbasis kriteria.  

> **Catatan:** File yang dibagikan di sini adalah versi demo. Jika ingin mendapatkan versi lengkap, dapat dibeli di [LYNK.ID KidouCode](https://lynk.id/kidoucode).

---

#### 📸 Preview Aplikasi

<p align="center">
  <img 
    src="https://pcobvoevxdmgjvpiorua.supabase.co/storage/v1/object/public/apps-spk-pemilihan-handphone-metode-saw/Screenshot%20Form%20Login.png"
    width="600"
    alt="Form Login"
  />
</p>

<p align="center">
  <img 
    src="https://pcobvoevxdmgjvpiorua.supabase.co/storage/v1/object/public/apps-spk-pemilihan-handphone-metode-saw/Screenshot%20Menu%20Utama.png"
    width="600"
    alt="Menu Utama"
  />
</p>

<p align="center">
  <img 
    src="https://pcobvoevxdmgjvpiorua.supabase.co/storage/v1/object/public/apps-spk-pemilihan-handphone-metode-saw/Screenshot%20Input%20Nilai%20Alternatif%20Per%20Kriteria.png"
    width="600"
    alt="Input Nilai Alternatif per Kriteria (SAW)"
  />
</p>


#### **Teknologi**
- [MySQL 8.0.40](https://downloads.mysql.com/archives/get/p/25/file/mysql-installer-community-8.0.40.0.msi)  
- [JDK 11](https://www.oracle.com/id/java/technologies/javase/jdk11-archive-downloads.html)  

Untuk menjalankan versi demo, cukup menggunakan **JDK 11**, karena database sudah di-host secara online.  
Namun, koneksi ke database mungkin mengalami keterlambatan.

---

#### **Library / Dependensi**

- **FlatLaf (Java Look and Feel)**  
  - `flatlaf-3.5.2.jar` → Tema modern Java Swing  
  - `flatlaf-3.5.2-sources.jar` → Source code untuk referensi/debug  
  - `flatlaf-extras-3.5.2.jar` → Fitur tambahan seperti custom accent color, font, dan icon  
  - `flatlaf-fonts-roboto-2.137.jar` → Font Roboto bawaan  
  - `flatlaf-intellij-themes-3.2.5.jar` → Tema mirip IntelliJ IDEA  
  - `jsvg-1.4.0.jar` → Render gambar SVG untuk icon  

- **MigLayout**  
  - `miglayout-core-5.3.jar` → Layout manager inti  
  - `miglayout-swing-5.3.jar` → Integrasi untuk Swing  

- **Modal Dialog**  
  - `modal-dialog-2.1.0.jar` → Dialog kustom dengan animasi  
  - `modal-dialog-demo-2.1.0.jar` → Contoh penggunaan  

- **MySQL Driver**  
  - `mysql-connector-j-8.0.31.jar` → JDBC driver MySQL  

- **Hashing**  
  - `jbcrypt-0.4.jar` → Hash password dengan BCrypt  

- **Jasper Report**  
  - `commons-beanutils-1.9.4.jar` → Utility untuk manipulasi properti JavaBean.
  - `commons-collections4-4.4.jar` → Struktur data koleksi tambahan.
  - `commons-digester-1.7.jar` → Parsing XML menjadi objek Java dengan aturan tertentu.
  - `commons-logging-1.3.0.jar` → Abstraksi logging untuk berbagai framework log.
  - `groovy-4.0.16.jar` → Bahasa Groovy yang digunakan oleh JasperReports untuk ekspresi dinamis.
  - `jasperreports-6.20.6.jar` → Library utama JasperReports untuk membuat dan meng-generate laporan.
  - `jasperreports-fonts-7.0.1.jar` → Font tambahan untuk digunakan dalam laporan Jasper.
  - `openpdf-1.3.30.jar` → Library PDF open-source untuk export laporan Jasper ke format PDF.

---

#### **Fitur Utama**
- Input kriteria dan alternatif (handphone)
- Input nilai alternatif per kriteria
- Perhitungan mencari nilai max, min dan normalisasi
- Perhitungan preferensi dan Hasil ranking

---

#### **Arsitektur Proyek (Package)**
- **Config** : Menangani konfigurasi koneksi aplikasi dengan database.  
- **DAO** : Implementasi logika akses data ke database, termasuk penerapan antarmuka service.  
- **Form** : Mengatur dan menampilkan data dalam bentuk tabel.  
- **Form Input** : Mengatur tampilan dan fungsi form untuk input data.  
- **Icon & Img** : Menyimpan ikon dan gambar yang digunakan aplikasi.  
- **Main** : Mengatur tampilan dan logika menu utama aplikasi.  
- **Model** : Mewakili struktur entitas sesuai tabel database.
- **Service** : Menyimpan logika bisnis untuk operasi CRUD, menghubungkan DAO dan UI.  
- **TableModel** : Model tabel khusus untuk `JTable`.  
- **Theme** : Menangani tema warna, gaya, dan layout aplikasi.  
- **Util** : Berisi fungsi-fungsi utilitas umum.  
- **Report** : Menyimpan file .jrxml dan .jasper.

---

#### **Instalasi & Menjalankan Aplikasi**

**1. Clone Repository**
```sh
git clone https://github.com/kidoucode/apps-spk-pemilihan-handphone-metode-saw-desktop.git
```

**2. Masuk ke Direktori Proyek** :

```sh
cd apps-spk-pemilihan-handphone-metode-saw-desktop
```

**3. Jalankan Aplikasi** :
```sh
java -jar AppsSPKSAWHandphone.jar
```
Atau Anda bisa langsung mengklik file JAR untuk menjalankan demo aplikasi ini.

**4. Login ke Aplikasi** :
```sh
Username : admin
Password : admin
```
Terima kasih

