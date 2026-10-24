# Studi Ablasi RNN, LSTM, GRU vs ANN untuk Prediksi Trafik Seluler Milan

Tugas Workshop Deep Learning — Teknik Telekomunikasi, Institut Teknologi Sumatera (ITERA).

## Identitas

| Nama | NIM | Kelas |
|---|---|---|
| Helsa Anastasya | 124400009 | RA |

**Pengerjaan:** Individu  
**Lokasi kelompok:** Kode 9 — Corso Como  
**Lokasi acuan:** Duomo (grid 5060)

## Deskripsi Proyek

Proyek ini membandingkan model ANN, RNN, LSTM, dan GRU untuk memprediksi aktivitas internet seluler per jam menggunakan dataset Telecom Italia di Kota Milan.

Eksperimen mencakup studi ablasi terhadap tujuh faktor, yaitu panjang jendela, ukuran hidden, jumlah lapisan, learning rate, kelompok fitur, batch size, dan early stopping patience.

Sebanyak 348 percobaan tercatat, termasuk konfigurasi acuan, konfigurasi terbaik, dan pengujian generalisasi lokasi.

## Hasil Utama

- Pada konfigurasi acuan di Duomo, RNN memperoleh Test MAE terendah sebesar 229,6.
- Konfigurasi gabungan meningkatkan Validation MAE ANN dari 248,9 menjadi 212,4.
- Pada Corso Como, GRU dengan konfigurasi gabungan menghasilkan Test MAE terendah sebesar 111,3.
- Hasil menunjukkan bahwa penggabungan hyperparameter terbaik secara individual tidak selalu meningkatkan akurasi.

## File Proyek

- `tugas_ablasi.ipynb` — Notebook eksperimen dan output.
- `data/` — Dataset yang digunakan.
- `hasil/` — Hasil eksperimen dalam CSV dan grafik.
- `laporan-latex/` — Source LaTeX laporan IEEE.
- `Laporan_Ablasi_Helsa_Anastasya.pdf` — Laporan akhir.
- `pyproject.toml` dan `uv.lock` — Dependensi proyek.

## Cara Menjalankan

```bash
uv sync
uv run jupyter lab
```

Buka file `tugas_ablasi.ipynb`, lalu jalankan sel sesuai urutan.

## Penggunaan AI

ChatGPT digunakan sebagai alat bantu memahami instruksi, menangani kesalahan teknis, mendampingi pelaksanaan eksperimen, serta membantu penyusunan laporan. Hasil evaluasi diperoleh dari eksekusi eksperimen menggunakan JupyterLab.
