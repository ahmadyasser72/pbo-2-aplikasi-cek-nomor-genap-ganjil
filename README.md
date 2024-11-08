# Tugas 1 - Aplikasi Cek Nomor Genap/Ganjil ([screenshot](#screenshot))

Aplikasi Java Swing ini digunakan untuk mengecek apakah sebuah angka merupakan **genap**, **ganjil**, atau **bilangan prima**. Dibuat menggunakan NetBeans IDE dan GUI Swing, aplikasi ini memiliki antarmuka sederhana yang memungkinkan pengguna memasukkan angka, memvalidasinya, dan menampilkan hasilnya dalam dialog pop-up.

## Fitur
- **Cek apakah angka genap atau ganjil**: Menunjukkan apakah angka yang dimasukkan merupakan bilangan genap atau ganjil.
- **Cek bilangan prima**: Untuk bilangan ganjil, juga akan mengecek apakah angka tersebut merupakan bilangan prima.
- **Validasi input**: Memastikan hanya nilai numerik yang diterima.
- **Auto-clear saat fokus**: Menghapus input secara otomatis saat kotak input diklik, untuk pengalaman pengguna yang lebih baik.

## Persiapan Awal

### Prasyarat
- Java Development Kit (JDK) versi 8 atau lebih tinggi
- NetBeans IDE (atau IDE lain yang mendukung aplikasi Java Swing)

### Menjalankan Aplikasi
1. Clone atau unduh repositori kode sumber ini.
2. Buka proyek di NetBeans atau IDE Java pilihan kamu.
3. Jalankan kelas `JFrameAplikasiCekNomorGenapGanjil` untuk memulai aplikasi.

### Cara Penggunaan
1. **Masukkan angka** di kotak input yang disediakan.
2. Klik tombol **"Cek ganjil/genap/prima"** untuk melihat hasilnya:
   - Aplikasi akan menampilkan pop-up yang menunjukkan apakah angka tersebut:
     - **Genap** atau **Ganjil**.
     - Jika ganjil, aplikasi juga akan memeriksa apakah angka tersebut merupakan bilangan **prima**.
3. **Input tidak valid**: Jika nilai non-numerik dimasukkan, dialog kesalahan akan muncul meminta input berupa angka saja.

## Penjelasan Kode

### Fungsi Utama
- **Pengecekan Bilangan** (`jButton1ActionPerformed`):
  - Mengambil input angka yang dimasukkan pengguna.
  - Mengecek apakah angka genap atau ganjil, dan menambahkan "genap" atau "ganjil" pada output.
  - Memanggil `isPrime(int num)` untuk menentukan apakah angka tersebut prima dan menambahkan "dan prima" jika benar.

- **Pemeriksaan Bilangan Prima** (`isPrime`):
  - Mengembalikan `true` jika angka tersebut prima dengan memeriksa keterbagian sampai akar kuadratnya.

- **Validasi Input** (`jTextField1KeyTyped`):
  - Memastikan hanya input numerik dengan membatasi karakter input pada angka dan tombol backspace.

## Detail tugas

1. Deskripsi Program:

   - GUI terdiri dari JTextField untuk input angka dan tombol Cek
   - Saat tombol ditekan, program akan memvalidasi input dan menampilkan hasilnya pada JLabel

2. Komponen GUI: JFrame, JPanel, JLabel, JTextField, JButton

3. Logika Program: Kondisional (if-else), Validasi input

4. Events:

   - ActionListener untuk tombol Cek
   - KeyAdapter pada JTextField untuk membatasi input hanya angka

5. Variasi:

   - Tambahkan fitur untuk memeriksa apakah angka tersebut adalah bilangan prima
   - Gunakan JOptionPane untuk menampilkan pesan hasil dan error
   - Implementasikan FocusListener untuk membersihkan JTextField saat mendapatkan fokus

## Screenshot

Nama : Ahmad Yasser

NPM  : 2210010525

Kelas: 5A REGULER BJB TI

1. Tampilan awal
![image](https://github.com/user-attachments/assets/8b1881e9-3a13-4985-8a8f-24c1e0a23d0a)

2. Saat ketik bukan angka
![image](https://github.com/user-attachments/assets/db47cc9f-e869-49cb-a353-5750207381b9)

3. Klik cek dengan inputan 10 (genap dan bukan prima)
![image](https://github.com/user-attachments/assets/2db633ec-e55f-4985-9437-1feb427ea018)

4. Klik cek dengan inputan 25 (ganjil dan bukan prima)
![image](https://github.com/user-attachments/assets/ba142b74-7c66-47df-972f-f61e5e971346)

5. Klik cek dengan inputan 13 (ganjil dan prima)
![image](https://github.com/user-attachments/assets/86218e4e-cb7d-463e-9db1-5f9daded20ca)
