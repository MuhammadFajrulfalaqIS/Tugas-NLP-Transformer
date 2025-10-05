Dibuat oleh **Muhammad Fajrulfalaq Izzulfirdausyah Suryaprabandaru**

# Implementasi Transformer dari Nol dengan NumPy

Proyek ini adalah implementasi arsitektur **Decoder-Only Transformer** dari nol (*from scratch*) hanya dengan menggunakan **NumPy**. Tugas ini bertujuan untuk membangun dan memahami alur *forward pass* dari sebuah model Transformer tanpa bantuan *library deep learning* seperti PyTorch atau TensorFlow.

Implementasi ini dibuat secara modular sesuai dengan spesifikasi tugas dan disajikan dalam dua format:
1.  `transformer_from_scratch.py`: Skrip Python murni.
2.  `Tugas_Transformer.ipynb`: Jupyter Notebook dengan penjelasan detail, visualisasi, dan simulasi prediksi kata.

---

## 🧩 Komponen yang Diimplementasikan

Semua komponen wajib dari arsitektur Transformer telah berhasil diimplementasikan sesuai dengan deskripsi tugas:

- [x] **Token Embedding**: Representasi token sebagai vektor.
- [x] **Positional Encoding**: Penambahan informasi urutan menggunakan fungsi sinusoidal.
- [x] **Scaled Dot-Product Attention**: Mekanisme inti dari perhatian dengan *scaling*.
- [x] **Causal Masking**: Pencegahan token untuk melihat token di masa depan.
- [x] **Multi-Head Attention**: Implementasi perhatian dari berbagai "sudut pandang" secara paralel.
- [x] **Feed-Forward Network**: Jaringan dua lapis dengan aktivasi non-linear (GELU).
- [x] **Residual Connection + Layer Normalization**: Menggunakan struktur *pre-norm* untuk stabilitas.
- [x] **Output Layer**: Proyeksi akhir ke ukuran kosakata dan distribusi `softmax`.
- [x] **Bonus**: Visualisasi matriks perhatian (*attention matrix*) untuk membuktikan cara kerja *causal masking*.

---

## ⚙️ Dependensi

Dependensi utama untuk proyek ini sangat minimal, sesuai dengan aturan tugas.

* **Wajib**:
    * `numpy`
* **Opsional** (hanya untuk visualisasi di notebook `.ipynb`):
    * `matplotlib`

Anda dapat menginstal semua dependensi dengan menjalankan perintah berikut:

```bash
pip install numpy matplotlib
```

---

## 🚀 Cara Menjalankan Program

Ada dua cara untuk menjalankan kode ini, tergantung pada file yang Anda pilih.

### 1. Menggunakan Skrip Python (`transformer_from_scratch.py`)

Skrip ini berisi implementasi inti dan sebuah uji coba sederhana di bagian bawahnya.

1.  **Clone Repositori Ini**
    ```bash
    git clone https://github.com/MuhammadFajrulfalaqIS/Tugas-NLP-Transformer.git
    cd Tugas-NLP-Transformer
    ```

2.  **Instal Dependensi**
    ```bash
    pip install numpy
    ```

3.  **Jalankan Skrip**
    Untuk menghindari masalah jika Anda memiliki banyak versi Python, disarankan menggunakan perintah `py` (untuk Windows) atau `python3` (untuk macOS/Linux).

    ```bash
    # Untuk Windows
    py transformer_from_scratch.py

    # Untuk macOS / Linux
    python3 transformer_from_scratch.py
    ```
    Anda akan melihat output di terminal yang memverifikasi bentuk tensor dan hasil uji coba lainnya.

### 2. Menggunakan Jupyter Notebook (`Tugas_Transformer.ipynb`)

Notebook ini berisi penjelasan yang jauh lebih detail, visualisasi, dan simulasi prediksi kata. Ini adalah cara terbaik untuk memahami setiap komponen secara interaktif.

1.  **Pastikan Anda Memiliki Jupyter**
    Jika Anda belum punya, instal dengan `pip install notebook`. Anda juga bisa menggunakan ekstensi Jupyter di Visual Studio Code.

2.  **Jalankan Jupyter Notebook**
    Buka terminal, arahkan ke folder proyek, dan jalankan:
    ```bash
    jupyter notebook
    ```

3.  **Buka File dan Jalankan Sel**
    Di browser Anda, buka file `Tugas_Transformer.ipynb`. Jalankan setiap sel secara berurutan dari atas ke bawah untuk melihat semua penjelasan dan hasil eksekusi kode.

---

## ✍️ Penulis
