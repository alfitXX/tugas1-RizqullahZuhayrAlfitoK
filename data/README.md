# Data Tugas 1

## Dataset yang Dipilih

Isi informasi berikut sebelum Milestone 1.

| Item | Isi |
|---|---|
| Nama dataset | `[isi nama dataset]` |
| Sumber | `[URL BPS / Satu Data Indonesia / BMKG / HuggingFace / Kaggle]` |
| Lisensi/ketentuan pakai | `[isi]` |
| Ukuran | `[>= 500 MB atau > 1.000.000 baris]` |
| Periode data | `[isi]` |
| Unit analisis | `[isi]` |

## Tempat Mencari Dataset

Pilih dataset Indonesia yang legal digunakan, dapat didokumentasikan sumbernya, dan memenuhi batas ukuran tugas.

| Situs | Kegunaan |
|---|---|
| [Satu Data Indonesia](https://data.go.id/) | Portal data terbuka lintas instansi pemerintah Indonesia. |
| [Badan Pusat Statistik](https://www.bps.go.id/) | Statistik sosial, ekonomi, kependudukan, dan data wilayah. |
| [BMKG Data Online](https://dataonline.bmkg.go.id/) | Data cuaca, iklim, gempa bumi, dan observasi meteorologi. |
| [Hugging Face Datasets](https://huggingface.co/datasets) | Dataset publik yang dapat dicari berdasarkan topik, bahasa, atau ukuran. |
| [Kaggle Datasets](https://www.kaggle.com/datasets) | Katalog dataset publik; periksa lisensi dan dokumentasi pembuatnya. |
| [Google Dataset Search](https://datasetsearch.research.google.com/) | Mesin pencari untuk menemukan dataset dari berbagai portal. |

## Cara Memperoleh Data

1. Buka URL sumber di atas.
2. Unduh file ke folder `data/raw/` tanpa mengubah data mentah.
3. Catat nama file dan checksum bila tersedia.
4. Ubah variabel `DATA_PATH` pada `notebooks/01_data_profiling.ipynb` agar menunjuk ke file tersebut.

## Aturan Penyimpanan

- Jangan commit dataset mentah atau hasil olahan berukuran besar ke Git.
- File pada `data/raw/` adalah data asli dan tidak boleh diubah.
- Simpan hasil transformasi yang dapat direproduksi pada `data/processed/`.


# Data Tugas 1

## Dataset yang Dipilih

Isi informasi berikut sebelum Milestone 1.

| **Item**                | **Isi**                                                         |
| ----------------------- | --------------------------------------------------------------- |
| Nama dataset            | Indonesian News Dataset                                         |
| Sumber                  | [Kaggle – Indonesian News Dataset] (https://www.kaggle.com/datasets/iqbalmaulana/indonesian-news-dataset) |
| Lisensi/ketentuan pakai | Mengikuti lisensi dan ketentuan penggunaan yang tercantum pada halaman dataset Kaggle |
| Ukuran                  | Dataset berita berbahasa Indonesia dengan jumlah data yang memenuhi kebutuhan analisis tugas |
| Periode data            | Data berita Indonesia sesuai periode yang tersedia pada dataset |
| Unit analisis           | Artikel berita |

## Tempat Mencari Dataset

Dataset diperoleh dari **Kaggle Datasets**, yaitu katalog dataset publik yang dapat digunakan untuk kebutuhan analisis data dengan tetap memperhatikan lisensi dan ketentuan penggunaan dataset.

Sumber dataset:

[Indonesian News Dataset – Kaggle] (https://www.kaggle.com/datasets/iqbalmaulana/indonesian-news-dataset)

## Cara Memperoleh Data

1. Membuka halaman sumber dataset pada Kaggle.
2. Mengunduh dataset **Indonesian News Dataset**.
3. Menyimpan file dataset mentah ke folder `data/raw/` tanpa mengubah isi data asli.
4. Mencatat nama file dataset yang digunakan.
5. Mengubah variabel `DATA_PATH` pada `notebooks/01_data_profiling.ipynb` agar menunjuk ke file dataset yang telah disimpan.

## Aturan Penyimpanan

- Dataset mentah tidak diubah dan disimpan pada folder `data/raw/`.
- Dataset mentah atau hasil olahan berukuran besar tidak di-commit ke Git.
- Hasil transformasi dan data yang telah diproses disimpan pada folder `data/processed/`.
- Seluruh proses pengolahan data dibuat agar dapat direproduksi dari dataset mentah.