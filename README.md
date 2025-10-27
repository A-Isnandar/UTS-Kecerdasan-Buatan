# UTS Kecerdasan Buatan - Logika Fuzzy Tsukamoto

Repository ini berisi pengerjaan Ujian Tengah Semester (UTS) untuk mata kuliah Kecerdasan Buatan, dengan studi kasus penentuan jumlah produksi menggunakan _Fuzzy Inference System (FIS)_.

---

## Author

- **Nama** : Muhamad Ario Isnandar
- **Kelas** : 05TPLE013
- **NIM** : 231011401602
- **Program Studi** : Teknik Informatika
- **Mata Kuliah** : Kecerdasan Buatan

---

## 📝 Deskripsi Proyek

Proyek ini bertujuan untuk menyelesaikan studi kasus dari `Soal UTS.ipynb` mengenai penentuan jumlah produksi makanan kaleng (Jenis ABC) oleh sebuah perusahaan.

Penentuan jumlah produksi didasarkan pada dua variabel input:

1.  **Permintaan**
2.  **Persediaan**

Metode yang digunakan adalah **Logika Fuzzy dengan inferensi Tsukamoto**, sesuai dengan 6 aturan (rules) yang diberikan dalam soal.

---

## ⚙️ Implementasi dan Hasil

Solusi ini diimplementasikan dalam sebuah file Jupyter Notebook (`.ipynb`) yang mencakup keseluruhan proses:

1.  **Perhitungan Manual**: Penjelasan _step-by-step_ dalam format Markdown yang mencakup:
    - **Fuzzifikasi** (Mencari derajat keanggotaan μ)
    - **Inferensi Aturan** (Mencari nilai predikat α dan `z` dari tiap aturan)
    - **Defuzzifikasi** (Menggunakan metode _Weighted Average_ / Rata-rata Tertimbang)
2.  **Kode Program Python**: Implementasi kode untuk melakukan perhitungan yang sama secara otomatis.
3.  **Visualisasi Grafik**: Pembuatan grafik himpunan fuzzy untuk `Permintaan` dan `Persediaan` menggunakan Matplotlib, lengkap dengan plot fuzifikasi berdasarkan nilai input yang dipilih.

### Input yang Dipilih

Sesuai instruksi soal dan konfirmasi dosen, nilai input (crisp value) dipilih secara mandiri dari rentang yang diberikan:

- **Permintaan (X)**: `2069` (kemasan)
- **Persediaan (Y)**: `569` (kemasan)

### Hasil Akhir

Berdasarkan perhitungan manual dan eksekusi kode program, didapatkan hasil akhir:

- **Jumlah Produksi (Z)**: **4771 kemasan** (pembulatan dari 4770.9688...)

---

## 📚 Library yang Dibutuhkan

Proyek ini bergantung pada beberapa library Python yang esensial untuk analisis data dan visualisasi. Semua dependensi tercatat dalam file `requirements.txt`.

- **`jupyter`**: Untuk membuat dan menjalankan file notebook (.ipynb).
- **`matplotlib`**: Digunakan untuk membuat visualisasi/grafik himpunan fuzzy.
- **`numpy`**: Digunakan untuk membantu proses pembuatan data (range) untuk plot grafik.

---

## 🚀 Cara Menjalankan

Proyek ini disarankan untuk dijalankan menggunakan _virtual environment_ (`venv`) untuk menghindari konflik dependensi.

1.  **Clone repository ini:**

    ```bash
    git clone [URL_GITHUB_LU_DI_SINI]
    cd [NAMA_FOLDER_REPO_LU]
    ```

2.  **Buat dan aktifkan virtual environment:**

    ```bash
    # Membuat venv
    python -m venv venv

    # Aktivasi di Windows (CMD/PowerShell)
    .\venv\Scripts\activate

    # Aktivasi di MacOS/Linux (atau Git Bash di Windows)
    source venv/bin/activate
    ```

3.  **Install semua library yang dibutuhkan:**

    ```bash
    pip install -r requirements.txt
    ```

4.  **Jalankan Jupyter Notebook:**
    ```bash
    jupyter notebook [NAMA_FILE_ipynb_LU].ipynb
    ```
    Atau, buka file `.ipynb` tersebut langsung melalui VS Code yang sudah terinstall ekstensi Python dan Jupyter.
